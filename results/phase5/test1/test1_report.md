# Test 1: the five methods on the corrected base model

Methods: Method 1: Weighted-sum genetic algorithm (base paper); Method 2: Non-dominated Sorting Genetic Algorithm III (base paper); Method 3: CP-SAT alone (exact solver); Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning; Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning.

Runs per random method: 30; time limit 1500 s per run; one processor core per run; errors: 0.
Indicator: Tolerance 0 = best feasible F1 (%); Tolerance 1 = hypervolume of (F1, Z2), reference (60, 60).

## Results (indicator: mean, standard deviation, best, worst; and the measures of Section 4.2)

| configuration | tolerance | method | mean | sd | best | worst | runs | runs_with_value | feasibility_rate_percent | gap_to_upper_bound_percent | improvement_over_paper_percent | published_points_dominated_share | igd_to_best_known_front | max_F2 | time_s |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| S1_EXTREME_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 68.85 | 0.00 | 68.85 | 68.85 | 30 | 30 | 100.00 | 5.46 | - | - | - | 66.67 | 1500.43 |
| S1_EXTREME_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 68.85 | - | 68.85 | 68.85 | 1 | 1 | 100.00 | 5.46 | - | - | - | 66.67 | 751.00 |
| S1_EXTREME_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 22.39 | 0.00 | 22.39 | 22.39 | 30 | 13 | 43.33 | 69.25 | - | - | - | 20.00 | 38.18 |
| S1_EXTREME_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 22.39 | 0.00 | 22.39 | 22.39 | 30 | 8 | 26.67 | 69.25 | - | - | - | 20.00 | 46.41 |
| S1_EXTREME_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 68.85 | 0.00 | 68.85 | 68.85 | 30 | 30 | 100.00 | 5.46 | - | - | - | 66.67 | 1500.32 |
| S1_EXTREME_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 801.38 | 7.88 | 820.07 | 793.79 | 30 | 30 | 100.00 | - | - | - | 0.19 | 75.00 | 1500.45 |
| S1_EXTREME_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 872.62 | - | 872.62 | 872.62 | 1 | 1 | 100.00 | - | - | - | 0.00 | 75.00 | 759.40 |
| S1_EXTREME_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 43.33 | - | - | - | 5.84 | 20.00 | 57.83 |
| S1_EXTREME_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 30.00 | - | - | - | 5.84 | 20.00 | 71.68 |
| S1_EXTREME_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 801.38 | 7.88 | 820.07 | 793.79 | 30 | 30 | 100.00 | - | - | - | 0.19 | 75.00 | 1500.38 |
| S1_HARD_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.08 | 0.00 | 73.08 | 73.08 | 30 | 30 | 100.00 | 0.26 | 4.49 | - | - | 64.71 | 1500.38 |
| S1_HARD_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 73.08 | - | 73.08 | 73.08 | 1 | 1 | 100.00 | 0.26 | 4.49 | - | - | 64.71 | 751.70 |
| S1_HARD_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 65.99 | 2.54 | 70.52 | 59.85 | 30 | 30 | 100.00 | 9.94 | -5.64 | - | - | 57.26 | 80.60 |
| S1_HARD_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 64.84 | 4.22 | 69.17 | 48.75 | 30 | 30 | 100.00 | 11.51 | -7.29 | - | - | 55.60 | 121.20 |
| S1_HARD_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 73.08 | 0.00 | 73.08 | 73.08 | 30 | 30 | 100.00 | 0.26 | 4.49 | - | - | 64.71 | 1500.37 |
| S1_HARD_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1062.36 | 0.00 | 1062.36 | 1062.36 | 30 | 30 | 100.00 | - | 35.45 | 1.00 | 0.00 | 73.33 | 1500.63 |
| S1_HARD_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 1062.36 | - | 1062.36 | 1062.36 | 1 | 1 | 100.00 | - | 35.45 | 1.00 | 0.00 | 73.33 | 941.50 |
| S1_HARD_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 178.79 | 124.48 | 392.27 | 0.00 | 30 | 30 | 100.00 | - | -77.20 | 0.00 | 2.11 | 53.45 | 82.34 |
| S1_HARD_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 256.44 | 197.41 | 611.51 | 0.00 | 30 | 30 | 100.00 | - | -67.30 | 0.01 | 1.89 | 55.10 | 70.36 |
| S1_HARD_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 1062.36 | 0.00 | 1062.36 | 1062.36 | 30 | 30 | 100.00 | - | 35.45 | 1.00 | 0.00 | 73.33 | 1500.64 |
| S1_MEDIUM_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.49 | 0.00 | 73.49 | 73.49 | 30 | 30 | 100.00 | 0.21 | 1.99 | - | - | 61.50 | 1500.88 |
| S1_MEDIUM_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 73.49 | - | 73.49 | 73.49 | 1 | 1 | 100.00 | 0.21 | 1.99 | - | - | 62.50 | 752.10 |
| S1_MEDIUM_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 71.22 | 0.96 | 72.88 | 68.76 | 30 | 30 | 100.00 | 3.29 | -1.15 | - | - | 56.95 | 63.16 |
| S1_MEDIUM_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 71.08 | 0.83 | 72.23 | 68.74 | 30 | 30 | 100.00 | 3.48 | -1.35 | - | - | 55.53 | 117.63 |
| S1_MEDIUM_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 73.49 | 0.00 | 73.49 | 73.49 | 30 | 30 | 100.00 | 0.21 | 1.99 | - | - | 61.83 | 1500.40 |
| S1_MEDIUM_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1087.97 | 0.23 | 1088.07 | 1087.46 | 30 | 30 | 100.00 | - | 29.95 | 1.00 | 0.04 | 68.75 | 1500.86 |
| S1_MEDIUM_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 1079.84 | - | 1079.84 | 1079.84 | 1 | 1 | 100.00 | - | 28.98 | 1.00 | 0.06 | 68.75 | 760.10 |
| S1_MEDIUM_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 641.88 | 75.13 | 775.42 | 500.08 | 30 | 30 | 100.00 | - | -23.33 | 0.02 | 0.95 | 55.59 | 60.24 |
| S1_MEDIUM_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 605.87 | 182.97 | 807.77 | 0.00 | 30 | 30 | 100.00 | - | -27.63 | 0.03 | 1.00 | 55.24 | 92.14 |
| S1_MEDIUM_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 1087.97 | 0.23 | 1088.07 | 1087.46 | 30 | 30 | 100.00 | - | 29.95 | 1.00 | 0.04 | 68.75 | 1501.05 |
| S2_EXTREME_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 68.96 | 0.00 | 68.96 | 68.96 | 30 | 30 | 100.00 | 4.52 | - | - | - | 66.67 | 1500.26 |
| S2_EXTREME_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 68.96 | - | 68.96 | 68.96 | 1 | 1 | 100.00 | 4.52 | - | - | - | 66.67 | 751.10 |
| S2_EXTREME_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 17.27 | 4.38 | 22.92 | 14.45 | 30 | 6 | 20.00 | 76.08 | - | - | - | 15.00 | 42.10 |
| S2_EXTREME_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 14.45 | 0.00 | 14.45 | 14.45 | 30 | 5 | 16.67 | 80.00 | - | - | - | 12.50 | 48.24 |
| S2_EXTREME_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 68.96 | 0.00 | 68.96 | 68.96 | 30 | 30 | 100.00 | 4.52 | - | - | - | 66.67 | 1500.68 |
| S2_EXTREME_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 863.70 | 4.31 | 878.58 | 862.35 | 30 | 30 | 100.00 | - | - | - | 0.05 | 75.00 | 1501.43 |
| S2_EXTREME_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 878.58 | - | 878.58 | 878.58 | 1 | 1 | 100.00 | - | - | - | 0.00 | 75.00 | 765.70 |
| S2_EXTREME_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 16.67 | - | - | - | 7.04 | 14.00 | 70.82 |
| S2_EXTREME_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 20.00 | - | - | - | 7.08 | 13.75 | 85.77 |
| S2_EXTREME_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 863.70 | 4.31 | 878.58 | 862.35 | 30 | 30 | 100.00 | - | - | - | 0.05 | 75.00 | 1501.24 |
| S2_HARD_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.07 | 0.08 | 73.08 | 72.65 | 30 | 30 | 100.00 | 0.14 | 5.90 | - | - | 64.60 | 1500.27 |
| S2_HARD_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 73.08 | - | 73.08 | 73.08 | 1 | 1 | 100.00 | 0.12 | 5.92 | - | - | 66.67 | 751.30 |
| S2_HARD_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 65.41 | 2.50 | 69.39 | 60.88 | 30 | 30 | 100.00 | 10.61 | -5.20 | - | - | 55.97 | 115.53 |
| S2_HARD_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 65.69 | 1.88 | 70.67 | 61.24 | 30 | 30 | 100.00 | 10.22 | -4.79 | - | - | 56.27 | 72.46 |
| S2_HARD_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 73.08 | 0.00 | 73.08 | 73.06 | 30 | 30 | 100.00 | 0.12 | 5.92 | - | - | 64.67 | 1500.27 |
| S2_HARD_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1053.95 | 1.11 | 1055.48 | 1049.43 | 30 | 30 | 100.00 | - | 68.27 | 1.00 | 0.03 | 71.43 | 1500.66 |
| S2_HARD_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 1051.75 | - | 1051.75 | 1051.75 | 1 | 1 | 100.00 | - | 67.92 | 1.00 | 0.03 | 71.43 | 802.00 |
| S2_HARD_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 248.03 | 151.86 | 519.70 | 0.00 | 30 | 30 | 100.00 | - | -60.40 | 0.00 | 2.02 | 54.64 | 41.18 |
| S2_HARD_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 314.25 | 162.20 | 572.57 | 0.00 | 30 | 30 | 100.00 | - | -49.83 | 0.00 | 1.86 | 56.21 | 63.27 |
| S2_HARD_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 1053.94 | 0.98 | 1055.48 | 1051.40 | 30 | 30 | 100.00 | - | 68.27 | 1.00 | 0.03 | 71.43 | 1500.70 |
| S2_MEDIUM_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.60 | 0.02 | 73.60 | 73.51 | 30 | 30 | 100.00 | 0.01 | 3.05 | - | - | 60.08 | 1500.32 |
| S2_MEDIUM_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 73.60 | - | 73.60 | 73.60 | 1 | 1 | 100.00 | 0.00 | 3.05 | - | - | 60.00 | 214.70 |
| S2_MEDIUM_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 70.52 | 1.05 | 72.35 | 67.73 | 30 | 30 | 100.00 | 4.18 | -1.25 | - | - | 55.17 | 46.45 |
| S2_MEDIUM_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 70.20 | 1.62 | 72.62 | 66.99 | 30 | 30 | 100.00 | 4.63 | -1.71 | - | - | 53.99 | 69.39 |
| S2_MEDIUM_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 73.60 | 0.02 | 73.60 | 73.51 | 30 | 30 | 100.00 | 0.01 | 3.05 | - | - | 60.17 | 1500.30 |
| S2_MEDIUM_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1078.77 | 1.38 | 1082.94 | 1073.95 | 30 | 30 | 100.00 | - | 27.21 | 1.00 | 0.03 | 68.54 | 1501.20 |
| S2_MEDIUM_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 1083.67 | - | 1083.67 | 1083.67 | 1 | 1 | 100.00 | - | 27.79 | 1.00 | 0.00 | 68.75 | 759.60 |
| S2_MEDIUM_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 591.68 | 88.30 | 705.57 | 403.86 | 30 | 30 | 100.00 | - | -30.23 | 0.00 | 1.25 | 54.08 | 34.30 |
| S2_MEDIUM_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 651.61 | 79.51 | 748.53 | 446.47 | 30 | 30 | 100.00 | - | -23.16 | 0.00 | 1.08 | 55.27 | 53.03 |
| S2_MEDIUM_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 1078.52 | 1.47 | 1082.62 | 1073.95 | 30 | 30 | 100.00 | - | 27.18 | 1.00 | 0.03 | 68.47 | 1502.10 |
| S3_EXTREME_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 68.65 | 0.25 | 68.69 | 67.30 | 30 | 30 | 100.00 | 1.74 | - | - | - | 66.59 | 1500.51 |
| S3_EXTREME_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 68.69 | - | 68.69 | 68.69 | 1 | 1 | 100.00 | 1.68 | - | - | - | 66.67 | 752.40 |
| S3_EXTREME_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 11.19 | 3.44 | 13.82 | 6.91 | 30 | 21 | 70.00 | 83.99 | - | - | - | 9.52 | 75.67 |
| S3_EXTREME_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 13.82 | 0.00 | 13.82 | 13.82 | 30 | 14 | 46.67 | 80.22 | - | - | - | 11.76 | 108.75 |
| S3_EXTREME_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 68.65 | 0.25 | 68.69 | 67.30 | 30 | 30 | 100.00 | 1.74 | - | - | - | 66.59 | 1500.49 |
| S3_EXTREME_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 632.28 | 2.62 | 634.82 | 618.73 | 30 | 30 | 100.00 | - | 102.08 | 1.00 | 0.50 | 68.75 | 1500.96 |
| S3_EXTREME_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 643.71 | - | 643.71 | 643.71 | 1 | 1 | 100.00 | - | 105.73 | 1.00 | 0.00 | 68.75 | 778.30 |
| S3_EXTREME_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 50.00 | - | -100.00 | 0.00 | 26.24 | 9.80 | 77.51 |
| S3_EXTREME_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 60.00 | - | -100.00 | 0.00 | 26.24 | 9.80 | 105.25 |
| S3_EXTREME_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 632.28 | 2.62 | 634.82 | 618.73 | 30 | 30 | 100.00 | - | 102.08 | 1.00 | 0.50 | 68.75 | 1500.77 |
| S3_HARD_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 70.19 | 0.00 | 70.19 | 70.19 | 30 | 30 | 100.00 | 0.12 | 0.59 | - | - | 62.50 | 1500.64 |
| S3_HARD_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 70.19 | - | 70.19 | 70.19 | 1 | 1 | 100.00 | 0.12 | 0.59 | - | - | 62.50 | 751.90 |
| S3_HARD_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 68.82 | 0.96 | 69.90 | 65.74 | 30 | 30 | 100.00 | 2.06 | -1.36 | - | - | 60.51 | 53.58 |
| S3_HARD_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 68.57 | 1.05 | 70.17 | 66.25 | 30 | 30 | 100.00 | 2.42 | -1.72 | - | - | 59.93 | 80.29 |
| S3_HARD_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 70.19 | 0.00 | 70.19 | 70.19 | 30 | 30 | 100.00 | 0.12 | 0.59 | - | - | 62.50 | 1500.63 |
| S3_HARD_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 881.31 | 0.00 | 881.31 | 881.31 | 30 | 30 | 100.00 | - | 51.06 | 1.00 | 0.09 | 70.59 | 1501.78 |
| S3_HARD_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 881.06 | - | 881.06 | 881.06 | 1 | 1 | 100.00 | - | 51.02 | 1.00 | 0.09 | 70.59 | 819.10 |
| S3_HARD_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 501.91 | 55.29 | 592.26 | 352.83 | 30 | 30 | 100.00 | - | -13.97 | 0.00 | 0.62 | 59.88 | 84.47 |
| S3_HARD_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 577.18 | 46.77 | 649.53 | 452.05 | 30 | 30 | 100.00 | - | -1.07 | 0.00 | 0.42 | 61.33 | 140.85 |
| S3_HARD_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 881.23 | 0.41 | 881.31 | 879.09 | 30 | 30 | 100.00 | - | 51.05 | 1.00 | 0.09 | 70.59 | 1501.81 |
| S3_MEDIUM_TOL0 | 0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 70.54 | 0.00 | 70.54 | 70.54 | 30 | 30 | 100.00 | 0.10 | 0.27 | - | - | 60.00 | 1500.65 |
| S3_MEDIUM_TOL0 | 0 | Method 3: CP-SAT alone (exact solver) | 70.54 | - | 70.54 | 70.54 | 1 | 1 | 100.00 | 0.10 | 0.27 | - | - | 60.00 | 751.70 |
| S3_MEDIUM_TOL0 | 0 | Method 1: Weighted-sum genetic algorithm (base paper) | 70.18 | 0.20 | 70.46 | 69.63 | 30 | 30 | 100.00 | 0.61 | -0.23 | - | - | 57.15 | 84.28 |
| S3_MEDIUM_TOL0 | 0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 70.24 | 0.23 | 70.48 | 69.74 | 30 | 30 | 100.00 | 0.53 | -0.16 | - | - | 58.31 | 133.71 |
| S3_MEDIUM_TOL0 | 0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 70.53 | 0.03 | 70.54 | 70.37 | 30 | 30 | 100.00 | 0.11 | 0.26 | - | - | 59.88 | 1500.90 |
| S3_MEDIUM_TOL1 | 1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 902.75 | 0.29 | 902.94 | 902.31 | 30 | 30 | 100.00 | - | 10.70 | 0.69 | 0.13 | 67.08 | 1501.99 |
| S3_MEDIUM_TOL1 | 1 | Method 3: CP-SAT alone (exact solver) | 899.80 | - | 899.80 | 899.80 | 1 | 1 | 100.00 | - | 10.34 | 0.69 | 0.13 | 62.50 | 946.70 |
| S3_MEDIUM_TOL1 | 1 | Method 1: Weighted-sum genetic algorithm (base paper) | 604.74 | 15.63 | 625.49 | 570.30 | 30 | 30 | 100.00 | - | -25.84 | 0.00 | 0.59 | 57.21 | 111.21 |
| S3_MEDIUM_TOL1 | 1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 688.83 | 27.49 | 738.02 | 621.88 | 30 | 30 | 100.00 | - | -15.53 | 0.05 | 0.35 | 58.04 | 138.96 |
| S3_MEDIUM_TOL1 | 1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 902.72 | 0.47 | 902.94 | 900.67 | 30 | 30 | 100.00 | - | 10.70 | 0.69 | 0.13 | 67.08 | 1500.95 |

## Targets of Table 10 for our method

| configuration | CP-SAT status | CP-SAT upper bound | proof that no roster exists | our feasibility rate % | published F2 (max) | our max F2 (mean) | met: feasible roster (or proof that none exists) | met: least satisfied staff member higher than published | base value | our mean | our mean gap % | met: at least the published value | met: optimality gap 0 % | published points dominated % | met: front dominates every published point | met: higher hypervolume |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| S1_EXTREME_TOL0 | FEASIBLE | 72.83 | False | 100.00 | 61.54 | 66.67 | True | True | - | 68.85 | 5.46 | True | False | - | - | - |
| S1_EXTREME_TOL1 | FEASIBLE | 72.85 | False | 100.00 | 66.67 | 75.00 | True | True | 0.00 | 801.38 | - | - | - | - | False | True |
| S1_HARD_TOL0 | FEASIBLE | 73.27 | False | 100.00 | 62.50 | 64.71 | True | True | 69.94 | 73.08 | 0.26 | True | False | - | - | - |
| S1_HARD_TOL1 | FEASIBLE | 73.27 | False | 100.00 | 66.67 | 73.33 | True | True | 784.32 | 1062.36 | - | - | - | 100.00 | True | True |
| S1_MEDIUM_TOL0 | FEASIBLE | 73.64 | False | 100.00 | 61.54 | 61.83 | True | True | 72.05 | 73.49 | 0.21 | True | False | - | - | - |
| S1_MEDIUM_TOL1 | FEASIBLE | 73.66 | False | 100.00 | 61.54 | 68.75 | True | True | 837.23 | 1087.97 | - | - | - | 100.00 | True | True |
| S2_EXTREME_TOL0 | FEASIBLE | 72.23 | False | 100.00 | 62.50 | 66.67 | True | True | - | 68.96 | 4.52 | True | False | - | - | - |
| S2_EXTREME_TOL1 | FEASIBLE | 72.25 | False | 100.00 | 64.29 | 75.00 | True | True | 0.00 | 863.70 | - | - | - | - | False | True |
| S2_HARD_TOL0 | FEASIBLE | 73.17 | False | 100.00 | 61.54 | 64.67 | True | True | 68.99 | 73.08 | 0.12 | True | False | - | - | - |
| S2_HARD_TOL1 | FEASIBLE | 73.17 | False | 100.00 | 62.50 | 71.43 | True | True | 626.36 | 1053.94 | - | - | - | 100.00 | True | True |
| S2_MEDIUM_TOL0 | OPTIMAL | 73.60 | False | 100.00 | 56.25 | 60.17 | True | True | 71.42 | 73.60 | 0.01 | True | True | - | - | - |
| S2_MEDIUM_TOL1 | OPTIMAL | 73.60 | False | 100.00 | 62.50 | 68.47 | True | True | 848.02 | 1078.52 | - | - | - | 100.00 | True | True |
| S3_EXTREME_TOL0 | FEASIBLE | 69.86 | False | 100.00 | 66.67 | 66.59 | True | False | - | 68.65 | 1.74 | True | False | - | - | - |
| S3_EXTREME_TOL1 | FEASIBLE | 69.92 | False | 100.00 | 66.67 | 68.75 | True | True | 312.89 | 632.28 | - | - | - | 100.00 | True | True |
| S3_HARD_TOL0 | FEASIBLE | 70.27 | False | 100.00 | 62.50 | 62.50 | True | False | 69.77 | 70.19 | 0.12 | True | False | - | - | - |
| S3_HARD_TOL1 | FEASIBLE | 70.27 | False | 100.00 | 66.67 | 70.59 | True | True | 583.40 | 881.23 | - | - | - | 100.00 | True | True |
| S3_MEDIUM_TOL0 | FEASIBLE | 70.61 | False | 100.00 | 60.00 | 59.88 | True | False | 70.35 | 70.53 | 0.11 | True | False | - | - | - |
| S3_MEDIUM_TOL1 | FEASIBLE | 70.62 | False | 100.00 | 62.50 | 67.08 | True | True | 815.49 | 902.72 | - | - | - | 68.75 | False | True |

## Our method against each other method (Wilcoxon tests with Holm correction)

| configuration | compared_with | mean_ours | mean_other | p_value | p_holm | significant_5_percent |
|---|---|---|---|---|---|---|
| S1_EXTREME_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 68.8502 | 68.8502 | 1.0000 | 1.0000 | False |
| S1_EXTREME_TOL0 | Method 3: CP-SAT alone (exact solver) | 68.8502 | 68.8502 | 1.0000 | 1.0000 | False |
| S1_EXTREME_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 68.8502 | 22.3905 | 0.0000 | 0.0000 | True |
| S1_EXTREME_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 68.8502 | 22.3905 | 0.0000 | 0.0000 | True |
| S1_EXTREME_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 801.3810 | 801.3810 | 1.0000 | 1.0000 | False |
| S1_EXTREME_TOL1 | Method 3: CP-SAT alone (exact solver) | 801.3810 | 872.6230 | 0.0000 | 0.0000 | True |
| S1_EXTREME_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 801.3810 | 0.0000 | 0.0000 | 0.0000 | True |
| S1_EXTREME_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 801.3810 | 0.0000 | 0.0000 | 0.0000 | True |
| S1_HARD_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.0784 | 73.0784 | 1.0000 | 1.0000 | False |
| S1_HARD_TOL0 | Method 3: CP-SAT alone (exact solver) | 73.0784 | 73.0784 | 1.0000 | 1.0000 | False |
| S1_HARD_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 73.0784 | 65.9881 | 0.0000 | 0.0000 | True |
| S1_HARD_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 73.0784 | 64.8378 | 0.0000 | 0.0000 | True |
| S1_HARD_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1062.3630 | 1062.3630 | 1.0000 | 1.0000 | False |
| S1_HARD_TOL1 | Method 3: CP-SAT alone (exact solver) | 1062.3630 | 1062.3630 | 1.0000 | 1.0000 | False |
| S1_HARD_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 1062.3630 | 178.7900 | 0.0000 | 0.0000 | True |
| S1_HARD_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 1062.3630 | 256.4390 | 0.0000 | 0.0000 | True |
| S1_MEDIUM_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.4908 | 73.4908 | 1.0000 | 1.0000 | False |
| S1_MEDIUM_TOL0 | Method 3: CP-SAT alone (exact solver) | 73.4908 | 73.4908 | 1.0000 | 1.0000 | False |
| S1_MEDIUM_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 73.4908 | 71.2242 | 0.0000 | 0.0000 | True |
| S1_MEDIUM_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 73.4908 | 71.0842 | 0.0000 | 0.0000 | True |
| S1_MEDIUM_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1087.9716 | 1087.9716 | 0.9417 | 0.9417 | False |
| S1_MEDIUM_TOL1 | Method 3: CP-SAT alone (exact solver) | 1087.9716 | 1079.8434 | 0.0000 | 0.0000 | True |
| S1_MEDIUM_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 1087.9716 | 641.8833 | 0.0000 | 0.0000 | True |
| S1_MEDIUM_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 1087.9716 | 605.8719 | 0.0000 | 0.0000 | True |
| S2_EXTREME_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 68.9637 | 68.9637 | 1.0000 | 1.0000 | False |
| S2_EXTREME_TOL0 | Method 3: CP-SAT alone (exact solver) | 68.9637 | 68.9637 | 1.0000 | 1.0000 | False |
| S2_EXTREME_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 68.9637 | 17.2735 | 0.0000 | 0.0000 | True |
| S2_EXTREME_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 68.9637 | 14.4487 | 0.0000 | 0.0000 | True |
| S2_EXTREME_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 863.7026 | 863.7026 | 1.0000 | 1.0000 | False |
| S2_EXTREME_TOL1 | Method 3: CP-SAT alone (exact solver) | 863.7026 | 878.5769 | 0.0000 | 0.0000 | True |
| S2_EXTREME_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 863.7026 | 0.0000 | 0.0000 | 0.0000 | True |
| S2_EXTREME_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 863.7026 | 0.0000 | 0.0000 | 0.0000 | True |
| S2_HARD_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.0803 | 73.0653 | 0.3049 | 0.6098 | False |
| S2_HARD_TOL0 | Method 3: CP-SAT alone (exact solver) | 73.0803 | 73.0809 | 0.3173 | 0.6098 | False |
| S2_HARD_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 73.0803 | 65.4081 | 0.0000 | 0.0000 | True |
| S2_HARD_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 73.0803 | 65.6908 | 0.0000 | 0.0000 | True |
| S2_HARD_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1053.9438 | 1053.9516 | 1.0000 | 1.0000 | False |
| S2_HARD_TOL1 | Method 3: CP-SAT alone (exact solver) | 1053.9438 | 1051.7460 | 0.0000 | 0.0000 | True |
| S2_HARD_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 1053.9438 | 248.0267 | 0.0000 | 0.0000 | True |
| S2_HARD_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 1053.9438 | 314.2514 | 0.0000 | 0.0000 | True |
| S2_MEDIUM_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 73.5951 | 73.5968 | 0.6998 | 0.6998 | False |
| S2_MEDIUM_TOL0 | Method 3: CP-SAT alone (exact solver) | 73.5951 | 73.6009 | 0.1573 | 0.3146 | False |
| S2_MEDIUM_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 73.5951 | 70.5241 | 0.0000 | 0.0000 | True |
| S2_MEDIUM_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 73.5951 | 70.1967 | 0.0000 | 0.0000 | True |
| S2_MEDIUM_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 1078.5237 | 1078.7741 | 0.2668 | 0.2668 | False |
| S2_MEDIUM_TOL1 | Method 3: CP-SAT alone (exact solver) | 1078.5237 | 1083.6671 | 0.0000 | 0.0000 | True |
| S2_MEDIUM_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 1078.5237 | 591.6777 | 0.0000 | 0.0000 | True |
| S2_MEDIUM_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 1078.5237 | 651.6078 | 0.0000 | 0.0000 | True |
| S3_EXTREME_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 68.6452 | 68.6452 | 1.0000 | 1.0000 | False |
| S3_EXTREME_TOL0 | Method 3: CP-SAT alone (exact solver) | 68.6452 | 68.6915 | 0.3173 | 0.6346 | False |
| S3_EXTREME_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 68.6452 | 11.1877 | 0.0000 | 0.0000 | True |
| S3_EXTREME_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 68.6452 | 13.8201 | 0.0000 | 0.0000 | True |
| S3_EXTREME_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 632.2849 | 632.2849 | 1.0000 | 1.0000 | False |
| S3_EXTREME_TOL1 | Method 3: CP-SAT alone (exact solver) | 632.2849 | 643.7100 | 0.0000 | 0.0000 | True |
| S3_EXTREME_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 632.2849 | 0.0000 | 0.0000 | 0.0000 | True |
| S3_EXTREME_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 632.2849 | 0.0000 | 0.0000 | 0.0000 | True |
| S3_HARD_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 70.1856 | 70.1856 | 1.0000 | 1.0000 | False |
| S3_HARD_TOL0 | Method 3: CP-SAT alone (exact solver) | 70.1856 | 70.1856 | 1.0000 | 1.0000 | False |
| S3_HARD_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 70.1856 | 68.8213 | 0.0000 | 0.0000 | True |
| S3_HARD_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 70.1856 | 68.5696 | 0.0000 | 0.0000 | True |
| S3_HARD_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 881.2346 | 881.3086 | 0.3337 | 0.3337 | False |
| S3_HARD_TOL1 | Method 3: CP-SAT alone (exact solver) | 881.2346 | 881.0603 | 0.0000 | 0.0000 | True |
| S3_HARD_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 881.2346 | 501.9140 | 0.0000 | 0.0000 | True |
| S3_HARD_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 881.2346 | 577.1805 | 0.0000 | 0.0000 | True |
| S3_MEDIUM_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 70.5330 | 70.5384 | 0.3337 | 0.6346 | False |
| S3_MEDIUM_TOL0 | Method 3: CP-SAT alone (exact solver) | 70.5330 | 70.5384 | 0.3173 | 0.6346 | False |
| S3_MEDIUM_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 70.5330 | 70.1822 | 0.0000 | 0.0000 | True |
| S3_MEDIUM_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 70.5330 | 70.2362 | 0.0000 | 0.0000 | True |
| S3_MEDIUM_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 902.7166 | 902.7530 | 0.9026 | 0.9026 | False |
| S3_MEDIUM_TOL1 | Method 3: CP-SAT alone (exact solver) | 902.7166 | 899.7950 | 0.0000 | 0.0000 | True |
| S3_MEDIUM_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 902.7166 | 604.7423 | 0.0000 | 0.0000 | True |
| S3_MEDIUM_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 902.7166 | 688.8289 | 0.0000 | 0.0000 | True |

## Friedman test across configurations, Tolerance 0

```
{
  "configurations": 9,
  "average_ranks": {
    "Method 1: Weighted-sum genetic algorithm (base paper)": 4.388888888888889,
    "Method 2: Non-dominated Sorting Genetic Algorithm III (base paper)": 4.611111111111111,
    "Method 3: CP-SAT alone (exact solver)": 1.6111111111111112,
    "Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning": 2.111111111111111,
    "Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning": 2.2777777777777777
  },
  "friedman_statistic": 32.05095541401273,
  "friedman_p": 1.8677673026821969e-06,
  "holm_p_vs_control": {
    "Method 2: Non-dominated Sorting Genetic Algorithm III (base paper)": 0.006980474798115921,
    "Method 1: Weighted-sum genetic algorithm (base paper)": 0.013862051890080052,
    "Method 3: CP-SAT alone (exact solver)": 0.7421867390453949,
    "Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning": 0.8230632737581216
  }
}
```

## Friedman test across configurations, Tolerance 1

```
{
  "configurations": 9,
  "average_ranks": {
    "Method 1: Weighted-sum genetic algorithm (base paper)": 4.722222222222222,
    "Method 2: Non-dominated Sorting Genetic Algorithm III (base paper)": 4.277777777777778,
    "Method 3: CP-SAT alone (exact solver)": 2.0,
    "Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning": 1.7777777777777777,
    "Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning": 2.2222222222222223
  },
  "friedman_statistic": 29.51479289940828,
  "friedman_p": 6.143680417741618e-06,
  "holm_p_vs_control": {
    "Method 1: Weighted-sum genetic algorithm (base paper)": 0.0031849206303631306,
    "Method 2: Non-dominated Sorting Genetic Algorithm III (base paper)": 0.017456619794299133,
    "Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning": 1.0,
    "Method 3: CP-SAT alone (exact solver)": 1.0
  }
}
```

