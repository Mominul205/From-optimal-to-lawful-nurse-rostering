# Test 2 (Option B): the improved model on a common grid

Methods: Method 1: Weighted-sum genetic algorithm (base paper); Method 2: Non-dominated Sorting Genetic Algorithm III (base paper); Method 3: CP-SAT alone (exact solver); Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning; Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning (Methods 1 and 2 adapted to the new rules; they use no grid).

Design: for each configuration the corner rosters of the front were computed once, with enough time, and the same grid of epsilon values on F2 and F3 was given to every run of Methods 3, 4 and 5; each grid point had the same time (time limit / number of points). Methods 1 and 2 runs are those of the original Test 2 (copied, unchanged) plus the runs that were missing. Errors: 0.

## Common grids

| configuration | eps_F2 | eps_F3 | grid_points | corners_found | computed_in_s |
|---|---|---|---|---|---|
| S1_TOL0 | [37.5, 47.2222, 56.9444, 66.6666] | [0] | 4 | 3 | 55.00 |
| S1_TOL1 | [43.75, 52.9761, 62.2023, 71.4285] | [0] | 4 | 3 | 123.10 |
| S2_TOL0 | [40.0, 48.0952, 56.1904, 64.2857] | [0] | 4 | 3 | 377.10 |
| S2_TOL1 | [50.0, 56.25, 62.5, 68.75] | [0] | 4 | 3 | 279.70 |
| S3_TOL0 | [50.0, 54.7619, 59.5238, 64.2857] | [0] | 4 | 3 | 263.70 |
| S3_TOL1 | [56.25, 60.4166, 64.5833, 68.75] | [0] | 4 | 3 | 542.20 |

## Results by method

| configuration | method | mean | sd | best | worst | runs | runs_with_value | feasibility_rate_percent | published_dominated_mean | time_s | igd_to_best_known_front | solved_points_mean |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| S1_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 0.00 | 0.00 | 189.35 | - | - |
| S1_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 0.00 | 0.00 | 199.02 | - | - |
| S1_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 10.00 | 0.00 | 228.89 | 23.49 | - |
| S1_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 3.33 | 0.00 | 253.60 | 18.30 | - |
| S2_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 33.33 | 0.00 | 367.27 | 16.93 | - |
| S2_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 20.00 | 0.00 | 226.85 | 14.75 | - |
| S2_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 16.67 | 0.00 | 190.60 | 32.77 | - |
| S2_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 26.67 | 0.00 | 454.27 | 27.69 | - |
| S3_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 50.00 | 0.00 | 366.15 | 22.95 | - |
| S3_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 30.00 | 0.00 | 598.80 | 19.71 | - |
| S3_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 70.00 | 0.00 | 174.54 | 47.24 | - |
| S3_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.00 | 0.00 | 0.00 | 0.00 | 30 | 30 | 53.33 | 0.00 | 147.64 | 41.11 | - |
| S1_TOL0 | Method 3: CP-SAT alone (exact solver) | 21538.95 | - | 21538.95 | 21538.95 | 1 | 1 | 100.00 | 4.00 | 151.00 | 0.00 | 4.00 |
| S1_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 21505.57 | 29.69 | 21538.95 | 21480.05 | 30 | 30 | 100.00 | 4.00 | 1493.12 | 0.01 | 4.00 |
| S1_TOL0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 21512.45 | 29.82 | 21538.95 | 21473.50 | 30 | 30 | 100.00 | 4.00 | 1491.64 | 0.01 | 4.00 |
| S1_TOL1 | Method 3: CP-SAT alone (exact solver) | 34249.31 | - | 34249.31 | 34249.31 | 1 | 1 | 100.00 | 6.00 | 180.60 | 0.00 | 4.00 |
| S1_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 34225.59 | 18.54 | 34249.31 | 34203.96 | 30 | 30 | 100.00 | 6.00 | 1493.20 | 0.02 | 4.00 |
| S1_TOL1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 34223.71 | 16.56 | 34249.31 | 34203.96 | 30 | 30 | 100.00 | 6.00 | 1493.75 | 0.02 | 4.00 |
| S2_TOL0 | Method 3: CP-SAT alone (exact solver) | 17682.61 | - | 17682.61 | 17682.61 | 1 | 1 | 100.00 | 2.00 | 726.00 | 0.00 | 4.00 |
| S2_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 17678.56 | 5.89 | 17682.61 | 17666.51 | 30 | 30 | 100.00 | 2.00 | 1496.25 | 0.00 | 4.00 |
| S2_TOL0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 17675.23 | 5.51 | 17682.61 | 17658.57 | 30 | 30 | 100.00 | 2.00 | 1496.38 | 0.00 | 4.00 |
| S2_TOL1 | Method 3: CP-SAT alone (exact solver) | 26778.46 | - | 26778.46 | 26778.46 | 1 | 1 | 100.00 | 5.00 | 1175.70 | 0.01 | 4.00 |
| S2_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 26784.85 | 5.19 | 26793.48 | 26771.35 | 30 | 30 | 100.00 | 5.00 | 1496.76 | 0.01 | 4.00 |
| S2_TOL1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 26786.63 | 5.46 | 26793.48 | 26771.35 | 30 | 30 | 100.00 | 5.00 | 1495.55 | 0.01 | 4.00 |
| S3_TOL0 | Method 3: CP-SAT alone (exact solver) | 15353.07 | - | 15353.07 | 15353.07 | 1 | 1 | 100.00 | 0.00 | 177.90 | 0.00 | 4.00 |
| S3_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 15348.69 | 3.70 | 15353.07 | 15339.10 | 30 | 30 | 100.00 | 0.00 | 1495.70 | 0.01 | 4.00 |
| S3_TOL0 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 15349.04 | 3.93 | 15353.07 | 15339.55 | 30 | 30 | 100.00 | 0.00 | 1495.80 | 0.01 | 4.00 |
| S3_TOL1 | Method 3: CP-SAT alone (exact solver) | 24997.94 | - | 24997.94 | 24997.94 | 1 | 1 | 100.00 | 4.00 | 1497.00 | 0.00 | 4.00 |
| S3_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 24994.23 | 4.40 | 24997.94 | 24983.44 | 30 | 30 | 100.00 | 4.00 | 1497.80 | 0.01 | 4.00 |
| S3_TOL1 | Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning | 24992.39 | 6.89 | 24997.94 | 24962.31 | 30 | 30 | 100.00 | 4.00 | 1495.89 | 0.01 | 4.00 |

## Table 11: published rosters against the rosters of our method

| measure | published_min | published_max | our_method_min | our_method_max |
|---|---|---|---|---|
| short_rest_periods | 35.00 | 86.00 | 0.00 | 0.00 |
| max_continuous_duty_hours | 12.00 | 24.00 | 8.00 | 12.00 |
| max_consecutive_working_days | 6.00 | 12.00 | 4.00 | 6.00 |
| staff_weeks_without_day_off | 0.00 | 3.00 | 0.00 | 0.00 |
| unwanted_share_percent | 24.88 | 33.87 | 28.13 | 32.48 |
| unwanted_spread | 5.00 | 10.00 | 2.00 | 3.00 |
| hours_share_min | 0.32 | 0.62 | 0.40 | 0.70 |
| hours_share_max | 0.60 | 1.00 | 0.56 | 0.84 |
| nights_spread | 5.00 | 11.00 | 1.00 | 2.00 |
| F3_total_shortage | 0.00 | 26.00 | 0.00 | 0.00 |
| F2_min_satisfaction_percent | 50.00 | 66.67 | 37.50 | 71.43 |
| F1_average_satisfaction_percent | 66.97 | 75.08 | 68.33 | 76.85 |

## Our method against each other method (Holm correction)

| configuration | compared_with | p_value | p_holm |
|---|---|---|---|
| S1_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.0000 | 0.0000 |
| S1_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.0000 | 0.0000 |
| S1_TOL0 | Method 3: CP-SAT alone (exact solver) | 0.0004 | 0.0007 |
| S1_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.6251 | 0.6251 |
| S1_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.0000 | 0.0000 |
| S1_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.0000 | 0.0000 |
| S1_TOL1 | Method 3: CP-SAT alone (exact solver) | 0.0000 | 0.0000 |
| S1_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.8017 | 0.8017 |
| S2_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.0000 | 0.0000 |
| S2_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.0000 | 0.0000 |
| S2_TOL0 | Method 3: CP-SAT alone (exact solver) | 0.0000 | 0.0000 |
| S2_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0212 | 0.0212 |
| S2_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.0000 | 0.0000 |
| S2_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.0000 | 0.0000 |
| S2_TOL1 | Method 3: CP-SAT alone (exact solver) | 0.0000 | 0.0000 |
| S2_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.0573 | 0.0573 |
| S3_TOL0 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.0000 | 0.0000 |
| S3_TOL0 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.0000 | 0.0000 |
| S3_TOL0 | Method 3: CP-SAT alone (exact solver) | 0.0001 | 0.0002 |
| S3_TOL0 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.6998 | 0.6998 |
| S3_TOL1 | Method 1: Weighted-sum genetic algorithm (base paper) | 0.0000 | 0.0000 |
| S3_TOL1 | Method 2: Non-dominated Sorting Genetic Algorithm III (base paper) | 0.0000 | 0.0000 |
| S3_TOL1 | Method 3: CP-SAT alone (exact solver) | 0.0000 | 0.0000 |
| S3_TOL1 | Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning | 0.2819 | 0.2819 |

## Friedman test

```
{
  "configurations": 6,
  "average_ranks": {
    "Method 1: Weighted-sum genetic algorithm (base paper)": 4.5,
    "Method 2: Non-dominated Sorting Genetic Algorithm III (base paper)": 4.5,
    "Method 3: CP-SAT alone (exact solver)": 1.3333333333333333,
    "Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning": 2.3333333333333335,
    "Method 5: Our method - Adaptive Large Neighbourhood Search + CP-SAT repair + Q-learning": 2.3333333333333335
  },
  "friedman_statistic": 20.631578947368418,
  "friedman_p": 0.00037462297987926754,
  "holm_p_vs_control": {
    "Method 1: Weighted-sum genetic algorithm (base paper)": 0.07048836384929746,
    "Method 2: Non-dominated Sorting Genetic Algorithm III (base paper)": 0.07048836384929746,
    "Method 3: CP-SAT alone (exact solver)": 0.5466433565845961,
    "Method 4: Adaptive Large Neighbourhood Search + CP-SAT repair, no learning": 1.0
  }
}
```
