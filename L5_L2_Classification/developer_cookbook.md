# Developer Cookbook — K_PHYAGENT
**Stack:** Python 3.11, PyTorch 2.10+, physics-informed neural nets, PAX 27B, AIOSS_FORMAT
**Domain:** PhyAgent: physics-informed agent for Anticloud embodied AI with real-world constraints

## Physics-constrained action planning
```python
from k_phyagent import PhyAgent

agent = PhyAgent(
    robot_urdf="./robot_description.urdf",
    pax_model="./pax-27b-q4.gguf",
    aioss_chain="./phyagent.aioss"
)

result = agent.plan_and_execute(
    task="Pick up the object on the left shelf",
    current_state=robot_state
)
print(f"Plan: {result.action_sequence}")
print(f"Physics valid: {result.all_actions_feasible}")
print(f"Energy cost: {result.estimated_energy:.2f}J")
```

## Check action feasibility
```python
feasible = agent.check_feasibility(
    action="move_joint_5 to 180 degrees at 100 rad/s"
)
print(f"Feasible: {feasible.ok}, reason: {feasible.reason}")
# Feasible: False, reason: velocity 100 rad/s exceeds joint_5 limit 3.14 rad/s
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
