# Step 17: scalability

Methods: Method 3: CP-SAT alone (exact solver); Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning; Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning.

Runs per search method: 10 (CP-SAT once: it is deterministic on one core); time limit 1500 s per run; 1 processor core(s) per run; the same starting roster for every method (the first feasible roster of CP-SAT); errors 0.
F1_after_t: best average satisfaction reached after t seconds (anytime performance).

| instance | staff | cores | model | method | final_F1_mean | final_F1_sd | best | worst | runs | start_F1 | gap_percent | verified_share | F1_after_60s | F1_after_300s | F1_after_900s | F1_after_1500s |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| L30_S1 | 30 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 75.67 | - | 75.67 | 75.67 | 1 | 61.24 | 0.00 | 1.00 | 75.67 | 75.67 | 75.67 | 75.67 |
| L30_S1 | 30 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 75.67 | 0.00 | 75.67 | 75.67 | 10 | 61.24 | 0.00 | 1.00 | 75.58 | 75.66 | 75.67 | 75.67 |
| L30_S1 | 30 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 75.67 | 0.00 | 75.67 | 75.67 | 10 | 61.24 | 0.00 | 1.00 | 75.58 | 75.66 | 75.67 | 75.67 |
| L30_S2 | 30 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 71.97 | - | 71.97 | 71.97 | 1 | 55.21 | 0.00 | 1.00 | 71.97 | 71.97 | 71.97 | 71.97 |
| L30_S2 | 30 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 71.97 | 0.00 | 71.97 | 71.97 | 10 | 55.21 | 0.00 | 1.00 | 71.78 | 71.97 | 71.97 | 71.97 |
| L30_S2 | 30 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 71.97 | 0.00 | 71.97 | 71.97 | 10 | 55.21 | 0.00 | 1.00 | 71.82 | 71.97 | 71.97 | 71.97 |
| L30_S3 | 30 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 71.38 | - | 71.38 | 71.38 | 1 | 59.97 | 0.00 | 1.00 | 71.12 | 71.38 | 71.38 | 71.38 |
| L30_S3 | 30 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 71.37 | 0.00 | 71.38 | 71.37 | 10 | 59.97 | 0.00 | 1.00 | 71.29 | 71.37 | 71.37 | 71.37 |
| L30_S3 | 30 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 71.37 | 0.00 | 71.38 | 71.36 | 10 | 59.97 | 0.01 | 1.00 | 71.13 | 71.37 | 71.37 | 71.37 |
| L60_S1 | 60 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 76.77 | - | 76.77 | 76.77 | 1 | 62.53 | 2.32 | 1.00 | 62.53 | 75.64 | 76.76 | 76.77 |
| L60_S1 | 60 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 76.84 | 0.00 | 76.85 | 76.84 | 10 | 62.53 | 2.21 | 1.00 | 75.34 | 76.79 | 76.83 | 76.84 |
| L60_S1 | 60 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 76.84 | 0.03 | 76.85 | 76.77 | 10 | 62.53 | 2.22 | 1.00 | 74.56 | 76.73 | 76.83 | 76.84 |
| L60_S2 | 60 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 74.02 | - | 74.02 | 74.02 | 1 | 58.39 | 4.81 | 1.00 | 58.39 | 58.39 | 59.43 | 74.02 |
| L60_S2 | 60 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 74.89 | 0.00 | 74.90 | 74.89 | 10 | 58.39 | 3.69 | 1.00 | 69.82 | 74.75 | 74.87 | 74.89 |
| L60_S2 | 60 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 74.88 | 0.03 | 74.90 | 74.80 | 10 | 58.39 | 3.70 | 1.00 | 70.02 | 74.60 | 74.86 | 74.88 |
| L60_S3 | 60 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 73.73 | - | 73.73 | 73.73 | 1 | 62.31 | 5.01 | 1.00 | 62.31 | 69.21 | 73.29 | 73.73 |
| L60_S3 | 60 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 74.00 | 0.06 | 74.05 | 73.87 | 10 | 62.31 | 4.66 | 1.00 | 68.95 | 73.70 | 73.95 | 74.00 |
| L60_S3 | 60 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 74.01 | 0.06 | 74.05 | 73.86 | 10 | 62.31 | 4.64 | 1.00 | 70.21 | 73.55 | 73.99 | 74.01 |
| L100_S1 | 100 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 76.56 | - | 76.56 | 76.56 | 1 | 61.24 | 3.01 | 1.00 | 61.24 | 61.24 | 74.80 | 76.56 |
| L100_S1 | 100 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 77.84 | 0.09 | 77.97 | 77.69 | 10 | 61.24 | 1.39 | 1.00 | 68.70 | 76.65 | 77.82 | 77.84 |
| L100_S1 | 100 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 77.87 | 0.08 | 77.98 | 77.72 | 10 | 61.24 | 1.36 | 1.00 | 70.61 | 76.13 | 77.80 | 77.87 |
| L100_S2 | 100 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 72.44 | - | 72.44 | 72.44 | 1 | 57.84 | 5.57 | 1.00 | 57.84 | 57.84 | 70.79 | 72.44 |
| L100_S2 | 100 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.90 | 0.28 | 74.24 | 73.23 | 10 | 57.84 | 3.66 | 1.00 | 61.34 | 67.72 | 73.24 | 73.90 |
| L100_S2 | 100 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 74.21 | 0.12 | 74.46 | 74.06 | 10 | 57.84 | 3.25 | 1.00 | 63.26 | 70.72 | 73.92 | 74.21 |
| L100_S3 | 100 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 57.59 | - | 57.59 | 57.59 | 1 | 57.59 | 21.50 | 1.00 | 57.59 | 57.59 | 57.59 | 57.59 |
| L100_S3 | 100 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 70.15 | 0.28 | 70.54 | 69.65 | 10 | 57.59 | 4.38 | 1.00 | 58.48 | 63.06 | 69.30 | 70.15 |
| L100_S3 | 100 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 70.31 | 0.51 | 71.09 | 69.46 | 10 | 57.59 | 4.16 | 1.00 | 60.12 | 65.74 | 69.36 | 70.31 |
| L150_S1 | 150 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 66.89 | - | 66.89 | 66.89 | 1 | 62.75 | 15.57 | 1.00 | 62.75 | 62.75 | 66.89 | 66.89 |
| L150_S1 | 150 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 76.65 | 0.76 | 77.25 | 75.42 | 10 | 62.75 | 3.24 | 1.00 | 67.29 | 73.53 | 76.42 | 76.65 |
| L150_S1 | 150 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 77.24 | 0.05 | 77.32 | 77.17 | 10 | 62.75 | 2.50 | 1.00 | 70.40 | 75.84 | 77.13 | 77.24 |
| L150_S2 | 150 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 70.04 | - | 70.04 | 70.04 | 1 | 59.91 | 9.09 | 1.00 | 59.91 | 59.91 | 59.91 | 70.04 |
| L150_S2 | 150 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 74.33 | 0.14 | 74.55 | 74.06 | 10 | 59.91 | 3.52 | 1.00 | 62.09 | 67.56 | 73.62 | 74.33 |
| L150_S2 | 150 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 74.43 | 0.51 | 74.91 | 73.41 | 10 | 59.91 | 3.40 | 1.00 | 62.48 | 68.97 | 73.45 | 74.43 |
| L150_S3 | 150 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 59.09 | - | 59.09 | 59.09 | 1 | 59.09 | 21.43 | 1.00 | 59.09 | 59.09 | 59.09 | 59.09 |
| L150_S3 | 150 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 70.17 | 1.16 | 71.33 | 67.40 | 10 | 59.09 | 6.70 | 1.00 | 59.97 | 63.76 | 68.33 | 70.17 |
| L150_S3 | 150 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 70.66 | 0.86 | 71.73 | 68.81 | 10 | 59.09 | 6.04 | 1.00 | 60.65 | 64.88 | 68.76 | 70.66 |
| L200_S1 | 200 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 71.05 | - | 71.05 | 71.05 | 1 | 61.11 | 7.00 | 1.00 | 61.11 | 61.11 | 61.11 | 71.05 |
| L200_S1 | 200 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 74.93 | 0.19 | 75.12 | 74.54 | 10 | 61.11 | 1.92 | 1.00 | 64.51 | 69.56 | 74.15 | 74.93 |
| L200_S1 | 200 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 74.87 | 0.46 | 75.15 | 73.83 | 10 | 61.11 | 2.00 | 1.00 | 65.61 | 71.48 | 74.05 | 74.87 |
| L200_S2 | 200 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 62.38 | - | 62.38 | 62.38 | 1 | 62.38 | 19.56 | 1.00 | 62.38 | 62.38 | 62.38 | 62.38 |
| L200_S2 | 200 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 71.55 | 1.14 | 72.70 | 68.71 | 10 | 62.38 | 7.73 | 1.00 | 63.47 | 66.53 | 70.35 | 71.55 |
| L200_S2 | 200 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 73.17 | 0.62 | 74.04 | 72.22 | 10 | 62.38 | 5.64 | 1.00 | 63.78 | 68.35 | 71.42 | 73.17 |
| L200_S3 | 200 | 1 | improved | Method 3: CP-SAT alone (exact solver) | 61.97 | - | 61.97 | 61.97 | 1 | 61.97 | 18.15 | 1.00 | 61.97 | 61.97 | 61.97 | 61.97 |
| L200_S3 | 200 | 1 | improved | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 64.43 | 1.96 | 68.77 | 62.43 | 10 | 61.97 | 14.90 | 1.00 | 62.34 | 63.22 | 64.10 | 64.43 |
| L200_S3 | 200 | 1 | improved | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 64.35 | 2.48 | 70.49 | 62.31 | 10 | 61.97 | 15.01 | 1.00 | 62.15 | 62.72 | 63.61 | 64.35 |

## Our method against each other method, final F1 (Holm correction)

| instance | model | cores | compared_with | p_value | p_holm |
|---|---|---|---|---|---|
| L30_S1 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 1.0000 | 1.0000 |
| L30_S1 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1.0000 | 1.0000 |
| L30_S2 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 1.0000 | 1.0000 |
| L30_S2 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1.0000 | 1.0000 |
| L30_S3 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0039 | 0.0078 |
| L30_S3 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0990 | 0.0990 |
| L60_S1 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L60_S1 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.8143 | 0.8143 |
| L60_S2 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L60_S2 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.7305 | 0.7305 |
| L60_S3 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L60_S3 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.6187 | 0.6187 |
| L100_S1 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L100_S1 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.5205 | 0.5205 |
| L100_S2 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0034 |
| L100_S2 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0017 | 0.0034 |
| L100_S3 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L100_S3 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.2730 | 0.2730 |
| L150_S1 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L150_S1 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0036 | 0.0039 |
| L150_S2 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L150_S2 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0257 | 0.0257 |
| L150_S3 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L150_S3 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.2730 | 0.2730 |
| L200_S1 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L200_S1 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.3447 | 0.3447 |
| L200_S2 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0020 |
| L200_S2 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0006 | 0.0012 |
| L200_S3 | improved | 1 | Method 3: CP-SAT alone (exact solver) | 0.0020 | 0.0039 |
| L200_S3 | improved | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.5205 | 0.5205 |

## Time to reach the result

Best known value: the best final F1 of all runs of all methods on the hospital (the proven optimum when CP-SAT proved it). Times in seconds from the common starting roster: median over the runs, where a run that never reached the target counts as slower than every other run ('not reached' when at least half of the runs did not reach it). Last improvement: when the final result of the run was found.

| instance | staff | model | cores | method | runs | best_known_F1 | best_known_is_proven_optimum | time_to_best_known_reached | median_time_to_best_known_s | time_to_within_0.5_percent_reached | median_time_to_within_0.5_percent_s | time_to_within_1_percent_reached | median_time_to_within_1_percent_s | median_time_last_improvement_s | cpsat_time_to_prove_optimum_s |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| L30_S1 | 30 | improved | 1 | CP-SAT | 1 | 75.67 | True | 1 of 1 | 40.5 | 1 of 1 | 35.2 | 1 of 1 | 33.9 | 40.47 | 55.8 |
| L30_S1 | 30 | improved | 1 | ALNS+CP-SAT | 10 | 75.67 | True | 10 of 10 | 316.9 | 10 of 10 | 20.7 | 10 of 10 | 14.6 | 316.92 | - |
| L30_S1 | 30 | improved | 1 | RL-ALNS+CP-SAT | 10 | 75.67 | True | 10 of 10 | 251.2 | 10 of 10 | 21.8 | 10 of 10 | 14.4 | 251.23 | - |
| L30_S2 | 30 | improved | 1 | CP-SAT | 1 | 71.97 | True | 1 of 1 | 55.4 | 1 of 1 | 50.1 | 1 of 1 | 40.9 | 55.42 | 72.0 |
| L30_S2 | 30 | improved | 1 | ALNS+CP-SAT | 10 | 71.97 | True | 10 of 10 | 75.2 | 10 of 10 | 35.4 | 10 of 10 | 26.7 | 75.17 | - |
| L30_S2 | 30 | improved | 1 | RL-ALNS+CP-SAT | 10 | 71.97 | True | 10 of 10 | 86.2 | 10 of 10 | 36.5 | 10 of 10 | 27.8 | 86.15 | - |
| L30_S3 | 30 | improved | 1 | CP-SAT | 1 | 71.38 | True | 1 of 1 | 119.4 | 1 of 1 | 51.9 | 1 of 1 | 43.7 | 119.39 | 423.4 |
| L30_S3 | 30 | improved | 1 | ALNS+CP-SAT | 10 | 71.38 | True | 4 of 10 | not reached | 10 of 10 | 31.9 | 10 of 10 | 25.6 | 123.68 | - |
| L30_S3 | 30 | improved | 1 | RL-ALNS+CP-SAT | 10 | 71.38 | True | 1 of 10 | not reached | 10 of 10 | 29.8 | 10 of 10 | 22.5 | 147.02 | - |
| L60_S1 | 60 | improved | 1 | CP-SAT | 1 | 76.85 | False | 0 of 1 | not reached | 1 of 1 | 577.5 | 1 of 1 | 426.8 | 1064.50 | not proven |
| L60_S1 | 60 | improved | 1 | ALNS+CP-SAT | 10 | 76.85 | False | 2 of 10 | not reached | 10 of 10 | 106.6 | 10 of 10 | 82.7 | 826.25 | - |
| L60_S1 | 60 | improved | 1 | RL-ALNS+CP-SAT | 10 | 76.85 | False | 3 of 10 | not reached | 10 of 10 | 128.3 | 10 of 10 | 88.8 | 1014.34 | - |
| L60_S2 | 60 | improved | 1 | CP-SAT | 1 | 74.90 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 1495.42 | not proven |
| L60_S2 | 60 | improved | 1 | ALNS+CP-SAT | 10 | 74.90 | False | 1 of 10 | not reached | 10 of 10 | 219.6 | 10 of 10 | 164.3 | 952.86 | - |
| L60_S2 | 60 | improved | 1 | RL-ALNS+CP-SAT | 10 | 74.90 | False | 2 of 10 | not reached | 10 of 10 | 224.5 | 10 of 10 | 151.2 | 732.40 | - |
| L60_S3 | 60 | improved | 1 | CP-SAT | 1 | 74.05 | False | 0 of 1 | not reached | 1 of 1 | 1,317.9 | 1 of 1 | 908.8 | 1496.91 | not proven |
| L60_S3 | 60 | improved | 1 | ALNS+CP-SAT | 10 | 74.05 | False | 1 of 10 | not reached | 10 of 10 | 301.5 | 10 of 10 | 191.9 | 1194.62 | - |
| L60_S3 | 60 | improved | 1 | RL-ALNS+CP-SAT | 10 | 74.05 | False | 2 of 10 | not reached | 10 of 10 | 251.8 | 10 of 10 | 167.1 | 654.01 | - |
| L100_S1 | 100 | improved | 1 | CP-SAT | 1 | 77.98 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 1430.67 | not proven |
| L100_S1 | 100 | improved | 1 | ALNS+CP-SAT | 10 | 77.98 | False | 0 of 10 | not reached | 10 of 10 | 488.6 | 10 of 10 | 407.7 | 1313.49 | - |
| L100_S1 | 100 | improved | 1 | RL-ALNS+CP-SAT | 10 | 77.98 | False | 1 of 10 | not reached | 10 of 10 | 601.8 | 10 of 10 | 365.8 | 1173.40 | - |
| L100_S2 | 100 | improved | 1 | CP-SAT | 1 | 74.46 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 1491.19 | not proven |
| L100_S2 | 100 | improved | 1 | ALNS+CP-SAT | 10 | 74.46 | False | 0 of 10 | not reached | 2 of 10 | not reached | 8 of 10 | 1,120.3 | 1433.41 | - |
| L100_S2 | 100 | improved | 1 | RL-ALNS+CP-SAT | 10 | 74.46 | False | 1 of 10 | not reached | 9 of 10 | 1,175.1 | 10 of 10 | 735.0 | 1422.05 | - |
| L100_S3 | 100 | improved | 1 | CP-SAT | 1 | 71.09 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 0.00 | not proven |
| L100_S3 | 100 | improved | 1 | ALNS+CP-SAT | 10 | 71.09 | False | 0 of 10 | not reached | 0 of 10 | not reached | 1 of 10 | not reached | 1455.60 | - |
| L100_S3 | 100 | improved | 1 | RL-ALNS+CP-SAT | 10 | 71.09 | False | 1 of 10 | not reached | 2 of 10 | not reached | 5 of 10 | not reached | 1468.07 | - |
| L150_S1 | 150 | improved | 1 | CP-SAT | 1 | 77.32 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 522.85 | not proven |
| L150_S1 | 150 | improved | 1 | ALNS+CP-SAT | 10 | 77.32 | False | 0 of 10 | not reached | 7 of 10 | 863.3 | 7 of 10 | 480.9 | 1315.29 | - |
| L150_S1 | 150 | improved | 1 | RL-ALNS+CP-SAT | 10 | 77.32 | False | 1 of 10 | not reached | 10 of 10 | 498.9 | 10 of 10 | 303.8 | 1332.48 | - |
| L150_S2 | 150 | improved | 1 | CP-SAT | 1 | 74.91 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 1423.22 | not proven |
| L150_S2 | 150 | improved | 1 | ALNS+CP-SAT | 10 | 74.91 | False | 0 of 10 | not reached | 2 of 10 | not reached | 9 of 10 | 1,320.0 | 1457.94 | - |
| L150_S2 | 150 | improved | 1 | RL-ALNS+CP-SAT | 10 | 74.91 | False | 1 of 10 | not reached | 8 of 10 | 1,318.2 | 8 of 10 | 976.1 | 1462.26 | - |
| L150_S3 | 150 | improved | 1 | CP-SAT | 1 | 71.73 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 0.00 | not proven |
| L150_S3 | 150 | improved | 1 | ALNS+CP-SAT | 10 | 71.73 | False | 0 of 10 | not reached | 0 of 10 | not reached | 3 of 10 | not reached | 1480.13 | - |
| L150_S3 | 150 | improved | 1 | RL-ALNS+CP-SAT | 10 | 71.73 | False | 1 of 10 | not reached | 3 of 10 | not reached | 3 of 10 | not reached | 1469.80 | - |
| L200_S1 | 200 | improved | 1 | CP-SAT | 1 | 75.15 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 1494.88 | not proven |
| L200_S1 | 200 | improved | 1 | ALNS+CP-SAT | 10 | 75.15 | False | 0 of 10 | not reached | 9 of 10 | 1,290.3 | 10 of 10 | 1,020.6 | 1475.23 | - |
| L200_S1 | 200 | improved | 1 | RL-ALNS+CP-SAT | 10 | 75.15 | False | 1 of 10 | not reached | 8 of 10 | 1,158.9 | 8 of 10 | 847.1 | 1471.30 | - |
| L200_S2 | 200 | improved | 1 | CP-SAT | 1 | 74.04 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 0.00 | not proven |
| L200_S2 | 200 | improved | 1 | ALNS+CP-SAT | 10 | 74.04 | False | 0 of 10 | not reached | 0 of 10 | not reached | 0 of 10 | not reached | 1457.60 | - |
| L200_S2 | 200 | improved | 1 | RL-ALNS+CP-SAT | 10 | 74.04 | False | 1 of 10 | not reached | 3 of 10 | not reached | 3 of 10 | not reached | 1489.56 | - |
| L200_S3 | 200 | improved | 1 | CP-SAT | 1 | 70.49 | False | 0 of 1 | not reached | 0 of 1 | not reached | 0 of 1 | not reached | 0.00 | not proven |
| L200_S3 | 200 | improved | 1 | ALNS+CP-SAT | 10 | 70.49 | False | 0 of 10 | not reached | 0 of 10 | not reached | 0 of 10 | not reached | 1229.53 | - |
| L200_S3 | 200 | improved | 1 | RL-ALNS+CP-SAT | 10 | 70.49 | False | 1 of 10 | not reached | 1 of 10 | not reached | 1 of 10 | not reached | 1475.55 | - |

## Our method against each other method, times (Holm correction)

| instance | model | cores | measure | compared_with | p_value | p_holm |
|---|---|---|---|---|---|---|
| L30_S1 | improved | 1 | time_to_best_known_s | CP-SAT | 0.0020 | 0.0039 |
| L30_S1 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.9698 | 0.9698 |
| L30_S1 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L30_S1 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.7337 | 0.7337 |
| L30_S1 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L30_S1 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.5708 | 0.5708 |
| L30_S2 | improved | 1 | time_to_best_known_s | CP-SAT | 0.0020 | 0.0039 |
| L30_S2 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3847 | 0.3847 |
| L30_S2 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.3223 | 0.6445 |
| L30_S2 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.7913 | 0.7913 |
| L30_S2 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0039 | 0.0078 |
| L30_S2 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.8501 | 0.8501 |
| L30_S3 | improved | 1 | time_to_best_known_s | CP-SAT | 0.0020 | 0.0039 |
| L30_S3 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.1012 | 0.1012 |
| L30_S3 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.5566 | 1.0000 |
| L30_S3 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 1.0000 | 1.0000 |
| L30_S3 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0488 | 0.0977 |
| L30_S3 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.4274 | 0.4274 |
| L60_S1 | improved | 1 | time_to_best_known_s | CP-SAT | 0.2500 | 0.5000 |
| L60_S1 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.8038 | 0.8038 |
| L60_S1 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L60_S1 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.2123 | 0.2123 |
| L60_S1 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L60_S1 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.3447 | 0.3447 |
| L60_S2 | improved | 1 | time_to_best_known_s | CP-SAT | 0.5000 | 1.0000 |
| L60_S2 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.6704 | 1.0000 |
| L60_S2 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L60_S2 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.9698 | 0.9698 |
| L60_S2 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L60_S2 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.8501 | 0.8501 |
| L60_S3 | improved | 1 | time_to_best_known_s | CP-SAT | 0.5000 | 1.0000 |
| L60_S3 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.5036 | 1.0000 |
| L60_S3 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L60_S3 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.2730 | 0.2730 |
| L60_S3 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L60_S3 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.8501 | 0.8501 |
| L100_S1 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L100_S1 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L100_S1 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L100_S1 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.3847 | 0.3847 |
| L100_S1 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L100_S1 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.8501 | 0.8501 |
| L100_S2 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L100_S2 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L100_S2 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0039 | 0.0059 |
| L100_S2 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.0030 | 0.0059 |
| L100_S2 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L100_S2 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.0058 | 0.0058 |
| L100_S3 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L100_S3 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L100_S3 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.5000 | 0.5000 |
| L100_S3 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.1681 | 0.3362 |
| L100_S3 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0625 | 0.1250 |
| L100_S3 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.0934 | 0.1250 |
| L150_S1 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L150_S1 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L150_S1 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L150_S1 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.0036 | 0.0039 |
| L150_S1 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0020 | 0.0039 |
| L150_S1 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.0139 | 0.0139 |
| L150_S2 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L150_S2 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L150_S2 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0078 | 0.0156 |
| L150_S2 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.0087 | 0.0156 |
| L150_S2 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0078 | 0.0156 |
| L150_S2 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.0535 | 0.0535 |
| L150_S3 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L150_S3 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L150_S3 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.2500 | 0.2500 |
| L150_S3 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.0779 | 0.1557 |
| L150_S3 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.2500 | 0.5000 |
| L150_S3 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.7093 | 0.7093 |
| L200_S1 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L200_S1 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L200_S1 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.0078 | 0.0156 |
| L200_S1 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.4720 | 0.4720 |
| L200_S1 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.0078 | 0.0156 |
| L200_S1 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.3073 | 0.3073 |
| L200_S2 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L200_S2 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L200_S2 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 0.2500 | 0.2500 |
| L200_S2 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.0779 | 0.1557 |
| L200_S2 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 0.2500 | 0.2500 |
| L200_S2 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.0779 | 0.1557 |
| L200_S3 | improved | 1 | time_to_best_known_s | CP-SAT | 1.0000 | 1.0000 |
| L200_S3 | improved | 1 | time_to_best_known_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L200_S3 | improved | 1 | time_to_within_0.5_percent_s | CP-SAT | 1.0000 | 1.0000 |
| L200_S3 | improved | 1 | time_to_within_0.5_percent_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
| L200_S3 | improved | 1 | time_to_within_1_percent_s | CP-SAT | 1.0000 | 1.0000 |
| L200_S3 | improved | 1 | time_to_within_1_percent_s | ALNS+CP-SAT | 0.3681 | 0.7362 |
