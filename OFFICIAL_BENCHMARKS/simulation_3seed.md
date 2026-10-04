# 3-Seed Simulation — K_PHYAGENT

**Seeds:** `18334` · `49671` · `83870`

**Seed method:** `sha256("K_PHYAGENT")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `K_PHYAGENT`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.0347 | 0.0151 | ±0.0296 |
| throughput_tokens_per_sec | 3387.9667 | 30.7827 | ±60.3341 |
| p50_latency_ms | 46.54 | 4.6103 | ±9.0362 |
| p99_latency_ms | 109.4567 | 1.5085 | ±2.9567 |
| ttft_ms | 29.1933 | 4.2379 | ±8.3063 |
| mmlu_proxy | 0.7592 | 0.0 | ±0.0 |
| hellaswag_proxy | 0.7601 | 0.0169 | ±0.0331 |
| truthfulqa_proxy | 0.5845 | 0.0146 | ±0.0286 |
| arc_proxy | 0.6844 | 0.0407 | ±0.0798 |
| complexity_cyclomatic | 4.4833 | 0.0377 | ±0.0739 |
| maintainability_index | 73.6133 | 4.1342 | ±8.103 |
| security_issues_high | 0.6667 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 77.8 | 2.5456 | ±4.9894 |
| test_coverage_pct | 62.7333 | 0.2357 | ±0.462 |
| doc_coverage_pct | 59.9333 | 2.3099 | ±4.5274 |
| memory_mb | 1674.1 | 58.407 | ±114.4777 |
| gpu_util_pct | 64.5 | 2.687 | ±5.2665 |
| openssf_score | 6.0267 | 0.6034 | ±1.1827 |
| eu_ai_act_compliance_pct | 82.0 | 0.5657 | ±1.1088 |
| slsa_level | 1.0 | 0.0 | ±0.0 |

## Per-Seed Raw Results

| Metric | Seed 18334 | Seed 49671 | Seed 83870 |
|--------|------------|------------|------------|
| trl_score | 7.024 | 7.056 | 7.024 |
| throughput_tokens_per_sec | 3366.2 | 3431.5 | 3366.2 |
| p50_latency_ms | 49.8 | 40.02 | 49.8 |
| p99_latency_ms | 108.39 | 111.59 | 108.39 |
| ttft_ms | 32.19 | 23.2 | 32.19 |
| mmlu_proxy | 0.7592 | 0.7592 | 0.7592 |
| hellaswag_proxy | 0.772 | 0.7362 | 0.772 |
| truthfulqa_proxy | 0.5948 | 0.5639 | 0.5948 |
| arc_proxy | 0.6556 | 0.7419 | 0.6556 |
| complexity_cyclomatic | 4.51 | 4.43 | 4.51 |
| maintainability_index | 70.69 | 79.46 | 70.69 |
| security_issues_high | 1 | 0 | 1 |
| dependency_freshness_pct | 76.0 | 81.4 | 76.0 |
| test_coverage_pct | 62.9 | 62.4 | 62.9 |
| doc_coverage_pct | 58.3 | 63.2 | 58.3 |
| memory_mb | 1715.4 | 1591.5 | 1715.4 |
| gpu_util_pct | 66.4 | 60.7 | 66.4 |
| openssf_score | 5.6 | 6.88 | 5.6 |
| eu_ai_act_compliance_pct | 81.6 | 82.8 | 81.6 |
| slsa_level | 1 | 1 | 1 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._