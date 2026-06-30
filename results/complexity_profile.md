# Complexity and Speed Profile

The table follows the manuscript profile before and after local-branch
re-parameterization. Values are reported as train-time / deploy-time.

| Input | Params (M) | Latency (ms) | Speedup | Peak memory (MB) | Memory reduction |
|---|---:|---:|---:|---:|---:|
| 256 x 256 | 8.880 / 4.744 | 28.24 / 11.96 | 2.36x | 2151.5 / 86.3 | 24.93x |
| 512 x 512 | 8.880 / 4.744 | 30.26 / 16.48 | 1.84x | 8447.9 / 256.4 | 32.95x |
| 1024 x 1024 | 8.880 / 4.744 | 82.08 / 69.69 | 1.18x | 17272.5 / 939.3 | 18.39x |

The deploy-time parameter count is used for the main quantitative table.
