# Ablation of our method

Runs per variant: 10; 120 s per run; one processor core.
p-values: full method against each variant (Holm correction within each instance).

| instance | variant | mean | sd | best | worst | runs | runs_with_value | p_value | p_holm |
|---|---|---|---|---|---|---|---|---|---|
| A1 | full (tuned) | 71.835 | 0.081 | 71.905 | 71.667 | 10 | 10 | - | - |
| A1 | no learning (roulette) | 71.855 | 0.066 | 71.905 | 71.758 | 10 | 10 | 0.239 | 1.000 |
| A1 | no adaptation (random) | 71.874 | 0.048 | 71.905 | 71.786 | 10 | 10 | 0.201 | 1.000 |
| A1 | without day_block | 71.845 | 0.081 | 71.905 | 71.667 | 10 | 10 | 0.848 | 1.000 |
| A1 | without fairness | 71.826 | 0.068 | 71.905 | 71.761 | 10 | 10 | 0.939 | 1.000 |
| A1 | without staffing | 71.850 | 0.065 | 71.905 | 71.773 | 10 | 10 | 0.510 | 1.000 |
| A1 | without random_staff | 71.763 | 0.087 | 71.905 | 71.626 | 10 | 10 | 0.063 | 0.438 |
| A1 | without workload | 71.859 | 0.090 | 71.905 | 71.629 | 10 | 10 | 0.262 | 1.000 |
| A2 | full (tuned) | 72.407 | 0.091 | 72.492 | 72.236 | 10 | 10 | - | - |
| A2 | no learning (roulette) | 72.381 | 0.133 | 72.507 | 72.059 | 10 | 10 | 0.791 | 1.000 |
| A2 | no adaptation (random) | 72.351 | 0.099 | 72.490 | 72.174 | 10 | 10 | 0.241 | 1.000 |
| A2 | without day_block | 72.061 | 0.201 | 72.362 | 71.718 | 10 | 10 | 0.000 | 0.002 |
| A2 | without fairness | 72.344 | 0.163 | 72.492 | 71.946 | 10 | 10 | 0.472 | 1.000 |
| A2 | without staffing | 72.292 | 0.198 | 72.482 | 71.891 | 10 | 10 | 0.121 | 0.727 |
| A2 | without random_staff | 72.285 | 0.283 | 72.492 | 71.672 | 10 | 10 | 1.000 | 1.000 |
| A2 | without workload | 72.319 | 0.158 | 72.502 | 72.047 | 10 | 10 | 0.364 | 1.000 |
| S1_TOL1 | full (tuned) | 76.537 | 0.000 | 76.537 | 76.537 | 10 | 10 | - | - |
| S1_TOL1 | no learning (roulette) | 76.536 | 0.005 | 76.537 | 76.521 | 10 | 10 | 0.368 | 1.000 |
| S1_TOL1 | no adaptation (random) | 76.537 | 0.000 | 76.537 | 76.537 | 10 | 10 | 1.000 | 1.000 |
| S1_TOL1 | without day_block | 76.536 | 0.005 | 76.537 | 76.521 | 10 | 10 | 0.368 | 1.000 |
| S1_TOL1 | without fairness | 76.537 | 0.000 | 76.537 | 76.537 | 10 | 10 | 1.000 | 1.000 |
| S1_TOL1 | without staffing | 76.535 | 0.006 | 76.537 | 76.519 | 10 | 10 | 0.368 | 1.000 |
| S1_TOL1 | without random_staff | 76.488 | 0.100 | 76.537 | 76.299 | 10 | 10 | 0.078 | 0.543 |
| S1_TOL1 | without workload | 76.537 | 0.000 | 76.537 | 76.537 | 10 | 10 | 1.000 | 1.000 |
