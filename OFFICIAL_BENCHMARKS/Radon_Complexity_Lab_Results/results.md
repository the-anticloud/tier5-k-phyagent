# Radon_Complexity_Lab_Results
**Project:** `K_PHYAGENT` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 4.452173913043478}`
- **complexity_grade:** `A`
- **complexity_score:** `4.452173913043478`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PHYAGENT\UPSTREAM\genesis\constants.py - A (100.00)
E:\fe`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PHYAGENT\UPSTREAM\genesis\constants.py
    C 17:0 IntEnum - A (2)
    C 174:0 backend - A (2)
    C 186:0 IMAGE_TYPE - A (2)
    M 18:4 IntEnum.__repr__ - A (1)
    M 21:4 IntEnum.__format__ - A (1)
    C 26:0 GEOM_TYPE - A (1)
    C 39:0 JOINT_TYPE - A (1)
    C 47:0 EQUALITY_TYPE - A (1)
    C 53:0 CTRL_MODE - A (1)
    C 61:0 integrator - A (1)
    C 68:0 constraint_solver - A (1)
    C 74:0 friction_cone - A (1)
    C 92:0 contact_resolution - A (1)
    C 121:0 broadphase_traversal - A (1)
    C 157:0 link_ref_frame - A (1)
    M 181:4 backend.__format__ - A (1)
    M 192:4 IMAGE_TYPE.__format__ - A (1)
    C 197:0 PARA_LEVEL - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PHYAGENT\UPSTREAM\genesis\datatypes.py
    M 79:4 List.__repr__colorized__ - C (14)
    M 63:4 List._repr_brief - B (6)
    C 19:0 List - A (4)
    M 27:4 List.__get_pydantic_core_schema__ - A (2)
    M 42:4 List.__getitem__ - A (2)
    M 53:4 List._repr_elem_colorized - A (2)
    M 37:4 List.__getitem__ - A (1)
    M 40:4 List.__getitem__ - A (1)
    M 48:4 List._repr_elem - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\K_PHYAGENT\UPSTREAM\genesis\repr_base.py
    M 16:4 RBC.__repr_name__ - B (7)
    M 51:4 RBC.__repr__colorized__ - B (7)
    C 8:0 RBC - A (4)
    M 44:4 RBC.__repr__ - A (4)
    M 36:4 RBC._repr_briefer - A (1)
    M 39:4 RBC._repr_brief - A (1)
    M 107:4 RBC.__format__ - A (1)
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_