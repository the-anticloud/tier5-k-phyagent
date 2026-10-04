# HF_Leaderboard_Lab_Results

**Project:** `K_PHYAGENT`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `Genesis-Embodied-AI/Genesis`  
**Commit:** `de8da45c91af`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **50.59 ms** |
| Min latency | 48.49 ms |
| Max latency | 55.48 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **41** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5858 |
| Classification latency | 121.47 ms |
| Status | **PASS** |

**Input text tokenized:**
```
K_PHYAGENT (Genesis-Embodied-AI/Genesis) — 1061 files, 197482 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'k', '_', 'ph', '##ya', '##gent', '(', 'genesis', '-', 'embodied', '-', 'ai', '/', 'genesis', ')', '—', '106', '##1', 'files', ',']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_