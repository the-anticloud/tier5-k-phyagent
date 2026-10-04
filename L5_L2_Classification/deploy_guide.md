# Deploy Guide — K_PHYAGENT
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, PyTorch 2.10+, physics-informed neural nets, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PyTorch 2.10+, T4 GPU for PINN inference. PAX 27B for task planning.

## Environment
T4 GPU. 16GB RAM. Robot description file (URDF) for physics model.

## AIOSS Integration
```bash
aioss init --module K_PHYAGENT --output ./k_phyagent.aioss
aioss append --chain ./k_phyagent.aioss --payload ./output.bin --module K_PHYAGENT
aioss verify --chain ./k_phyagent.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_PHYAGENT",
    aioss_chain="./K_PHYAGENT.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_PHYAGENT.aioss --verbose
python -m K_PHYAGENT.tests.smoke
```
