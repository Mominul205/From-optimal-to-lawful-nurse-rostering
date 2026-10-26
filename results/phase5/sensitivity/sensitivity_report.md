# Sensitivity: the price of rest and fairness

CP-SAT, 600 s per solve (maximise F1), started from the roster of the default model; F2 >= 60.0 %; Tolerance 1 with no shortage. Status OPTIMAL means proved optimal; FEASIBLE means the best roster found in the time (see F1_upper_bound in the runs table).
Price of a rule = F1 with the rule switched off - F1 with the rule (percentage points).

| scenario | tolerance | parameter | value | F1 | F1_rule_off | price_of_rule_points | change_vs_default_points |
|---|---|---|---|---|---|---|---|
| S1 | 0 | G_min_rest_hours | 8 | 71.65 | 73.64 | 2.00 | 0.00 |
| S1 | 0 | G_min_rest_hours | 10 | 71.65 | 73.64 | 2.00 | 0.00 |
| S1 | 0 | G_min_rest_hours | 11 | 71.65 | 73.64 | 2.00 | 0.00 |
| S1 | 0 | beta_hours_band | 0.05 | 71.63 | 71.65 | 0.02 | -0.02 |
| S1 | 0 | beta_hours_band | 0.1 | 71.65 | 71.65 | 0.00 | 0.00 |
| S1 | 0 | beta_hours_band | 0.15 | 71.65 | 71.65 | 0.00 | 0.00 |
| S1 | 0 | Theta_night_difference | 1 | 71.65 | 71.65 | 0.00 | 0.00 |
| S1 | 0 | Theta_night_difference | 2 | 71.65 | 71.65 | 0.00 | 0.00 |
| S1 | 0 | Theta_night_difference | 3 | 71.65 | 71.65 | 0.00 | 0.00 |
| S1 | 1 | G_min_rest_hours | 8 | 76.63 | 78.60 | 1.96 | 0.00 |
| S1 | 1 | G_min_rest_hours | 10 | 76.63 | 78.60 | 1.96 | 0.00 |
| S1 | 1 | G_min_rest_hours | 11 | 76.63 | 78.60 | 1.96 | 0.00 |
| S1 | 1 | beta_hours_band | 0.05 | 74.69 | 76.63 | 1.94 | -1.94 |
| S1 | 1 | beta_hours_band | 0.1 | 76.63 | 76.63 | 0.00 | 0.00 |
| S1 | 1 | beta_hours_band | 0.15 | 76.63 | 76.63 | 0.00 | 0.00 |
| S1 | 1 | Theta_night_difference | 1 | 76.62 | 76.63 | 0.02 | -0.02 |
| S1 | 1 | Theta_night_difference | 2 | 76.63 | 76.63 | 0.00 | 0.00 |
| S1 | 1 | Theta_night_difference | 3 | 76.63 | 76.63 | 0.00 | 0.00 |
| S2 | 0 | G_min_rest_hours | 8 | 70.58 | 73.48 | 2.90 | 0.51 |
| S2 | 0 | G_min_rest_hours | 10 | 70.07 | 73.48 | 3.41 | 0.00 |
| S2 | 0 | G_min_rest_hours | 11 | 70.07 | 73.48 | 3.41 | 0.00 |
| S2 | 0 | beta_hours_band | 0.05 | 70.07 | 70.07 | 0.00 | 0.00 |
| S2 | 0 | beta_hours_band | 0.1 | 70.07 | 70.07 | 0.00 | 0.00 |
| S2 | 0 | beta_hours_band | 0.15 | 70.07 | 70.07 | 0.00 | 0.00 |
| S2 | 0 | Theta_night_difference | 1 | 69.81 | 70.29 | 0.48 | -0.26 |
| S2 | 0 | Theta_night_difference | 2 | 70.07 | 70.29 | 0.22 | 0.00 |
| S2 | 0 | Theta_night_difference | 3 | 70.29 | 70.29 | 0.00 | 0.22 |
| S2 | 1 | G_min_rest_hours | 8 | 74.82 | 78.68 | 3.87 | 0.99 |
| S2 | 1 | G_min_rest_hours | 10 | 73.84 | 78.68 | 4.84 | 0.02 |
| S2 | 1 | G_min_rest_hours | 11 | 73.82 | 78.68 | 4.86 | 0.00 |
| S2 | 1 | beta_hours_band | 0.05 | 73.84 | 73.84 | 0.00 | 0.02 |
| S2 | 1 | beta_hours_band | 0.1 | 73.82 | 73.84 | 0.02 | 0.00 |
| S2 | 1 | beta_hours_band | 0.15 | 73.82 | 73.84 | 0.02 | 0.00 |
| S2 | 1 | Theta_night_difference | 1 | 73.60 | 74.29 | 0.68 | -0.22 |
| S2 | 1 | Theta_night_difference | 2 | 73.82 | 74.29 | 0.46 | 0.00 |
| S2 | 1 | Theta_night_difference | 3 | 74.06 | 74.29 | 0.22 | 0.24 |
| S3 | 0 | G_min_rest_hours | 8 | 69.71 | 70.74 | 1.03 | 0.84 |
| S3 | 0 | G_min_rest_hours | 10 | 68.87 | 70.74 | 1.87 | 0.00 |
| S3 | 0 | G_min_rest_hours | 11 | 68.87 | 70.74 | 1.87 | 0.00 |
| S3 | 0 | beta_hours_band | 0.05 | 68.85 | 68.87 | 0.02 | -0.02 |
| S3 | 0 | beta_hours_band | 0.1 | 68.87 | 68.87 | 0.00 | 0.00 |
| S3 | 0 | beta_hours_band | 0.15 | 68.87 | 68.87 | 0.00 | 0.00 |
| S3 | 0 | Theta_night_difference | 1 | 68.80 | 68.89 | 0.08 | -0.07 |
| S3 | 0 | Theta_night_difference | 2 | 68.87 | 68.89 | 0.02 | 0.00 |
| S3 | 0 | Theta_night_difference | 3 | 68.89 | 68.89 | 0.00 | 0.02 |
| S3 | 1 | G_min_rest_hours | 8 | 74.60 | 75.74 | 1.14 | 1.68 |
| S3 | 1 | G_min_rest_hours | 10 | 72.92 | 75.74 | 2.82 | 0.00 |
| S3 | 1 | G_min_rest_hours | 11 | 72.92 | 75.74 | 2.82 | 0.00 |
| S3 | 1 | beta_hours_band | 0.05 | 72.87 | 72.92 | 0.05 | -0.05 |
| S3 | 1 | beta_hours_band | 0.1 | 72.92 | 72.92 | 0.00 | 0.00 |
| S3 | 1 | beta_hours_band | 0.15 | 72.92 | 72.92 | 0.00 | 0.00 |
| S3 | 1 | Theta_night_difference | 1 | 72.90 | 73.18 | 0.28 | -0.03 |
| S3 | 1 | Theta_night_difference | 2 | 72.92 | 73.18 | 0.26 | 0.00 |
| S3 | 1 | Theta_night_difference | 3 | 73.18 | 73.18 | 0.00 | 0.26 |

## All runs

| scenario | tolerance | parameter | value | status | F1 | F2 | F3 | F1_upper_bound | short_rests | longest_duty_h | nights_spread | verified |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| S1 | 0 | (default model) | default | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 0 | G_min_rest_hours | 8 | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 0 | G_min_rest_hours | 10 | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 0 | G_min_rest_hours | off | OPTIMAL | 73.64 | 60.00 | 0 | 73.64 | 0 | 12.00 | 2 | True |
| S1 | 0 | beta_hours_band | 0.05 | OPTIMAL | 71.63 | 60.00 | 0 | 71.63 | 0 | 12.00 | 2 | True |
| S1 | 0 | beta_hours_band | 0.15 | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 0 | beta_hours_band | off | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 0 | Theta_night_difference | 1 | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 1 | True |
| S1 | 0 | Theta_night_difference | 3 | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 0 | Theta_night_difference | off | OPTIMAL | 71.65 | 60.00 | 0 | 71.65 | 0 | 12.00 | 2 | True |
| S1 | 1 | (default model) | default | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 2 | True |
| S1 | 1 | G_min_rest_hours | 8 | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 2 | True |
| S1 | 1 | G_min_rest_hours | 10 | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 2 | True |
| S1 | 1 | G_min_rest_hours | off | OPTIMAL | 78.60 | 60.00 | 0 | 78.60 | 0 | 12.00 | 2 | True |
| S1 | 1 | beta_hours_band | 0.05 | OPTIMAL | 74.69 | 60.00 | 0 | 74.69 | 0 | 12.00 | 2 | True |
| S1 | 1 | beta_hours_band | 0.15 | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 2 | True |
| S1 | 1 | beta_hours_band | off | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 2 | True |
| S1 | 1 | Theta_night_difference | 1 | OPTIMAL | 76.62 | 60.00 | 0 | 76.62 | 0 | 12.00 | 1 | True |
| S1 | 1 | Theta_night_difference | 3 | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 3 | True |
| S1 | 1 | Theta_night_difference | off | OPTIMAL | 76.63 | 60.00 | 0 | 76.63 | 0 | 12.00 | 2 | True |
| S2 | 0 | (default model) | default | OPTIMAL | 70.07 | 60.00 | 0 | 70.07 | 0 | 12.00 | 2 | True |
| S2 | 0 | G_min_rest_hours | 8 | OPTIMAL | 70.58 | 60.00 | 0 | 70.58 | 0 | 12.00 | 2 | True |
| S2 | 0 | G_min_rest_hours | 10 | OPTIMAL | 70.07 | 60.00 | 0 | 70.07 | 0 | 12.00 | 2 | True |
| S2 | 0 | G_min_rest_hours | off | OPTIMAL | 73.48 | 60.00 | 0 | 73.48 | 0 | 12.00 | 2 | True |
| S2 | 0 | beta_hours_band | 0.05 | OPTIMAL | 70.07 | 60.00 | 0 | 70.07 | 0 | 12.00 | 2 | True |
| S2 | 0 | beta_hours_band | 0.15 | OPTIMAL | 70.07 | 60.00 | 0 | 70.07 | 0 | 12.00 | 2 | True |
| S2 | 0 | beta_hours_band | off | OPTIMAL | 70.07 | 60.00 | 0 | 70.07 | 0 | 12.00 | 2 | True |
| S2 | 0 | Theta_night_difference | 1 | OPTIMAL | 69.81 | 60.00 | 0 | 69.81 | 0 | 12.00 | 1 | True |
| S2 | 0 | Theta_night_difference | 3 | OPTIMAL | 70.29 | 60.00 | 0 | 70.29 | 0 | 12.00 | 3 | True |
| S2 | 0 | Theta_night_difference | off | OPTIMAL | 70.29 | 60.00 | 0 | 70.29 | 0 | 12.00 | 6 | True |
| S2 | 1 | (default model) | default | FEASIBLE | 73.82 | 60.00 | 0 | 77.37 | 0 | 12.00 | 2 | True |
| S2 | 1 | G_min_rest_hours | 8 | OPTIMAL | 74.82 | 60.00 | 0 | 74.82 | 0 | 12.00 | 2 | True |
| S2 | 1 | G_min_rest_hours | 10 | FEASIBLE | 73.84 | 60.00 | 0 | 77.31 | 0 | 12.00 | 2 | True |
| S2 | 1 | G_min_rest_hours | off | OPTIMAL | 78.68 | 60.00 | 0 | 78.68 | 0 | 12.00 | 2 | True |
| S2 | 1 | beta_hours_band | 0.05 | OPTIMAL | 73.84 | 60.00 | 0 | 73.84 | 0 | 12.00 | 2 | True |
| S2 | 1 | beta_hours_band | 0.15 | FEASIBLE | 73.82 | 60.00 | 0 | 77.91 | 0 | 12.00 | 2 | True |
| S2 | 1 | beta_hours_band | off | FEASIBLE | 73.84 | 60.00 | 0 | 77.90 | 0 | 12.00 | 2 | True |
| S2 | 1 | Theta_night_difference | 1 | FEASIBLE | 73.60 | 60.00 | 0 | 77.36 | 0 | 12.00 | 1 | True |
| S2 | 1 | Theta_night_difference | 3 | OPTIMAL | 74.06 | 60.00 | 0 | 74.06 | 0 | 12.00 | 3 | True |
| S2 | 1 | Theta_night_difference | off | OPTIMAL | 74.29 | 60.00 | 0 | 74.29 | 0 | 12.00 | 6 | True |
| S3 | 0 | (default model) | default | OPTIMAL | 68.87 | 60.00 | 0 | 68.87 | 0 | 8.00 | 2 | True |
| S3 | 0 | G_min_rest_hours | 8 | OPTIMAL | 69.71 | 60.00 | 0 | 69.71 | 0 | 8.00 | 2 | True |
| S3 | 0 | G_min_rest_hours | 10 | OPTIMAL | 68.87 | 60.00 | 0 | 68.87 | 0 | 8.00 | 2 | True |
| S3 | 0 | G_min_rest_hours | off | OPTIMAL | 70.74 | 60.00 | 0 | 70.74 | 0 | 12.00 | 2 | True |
| S3 | 0 | beta_hours_band | 0.05 | OPTIMAL | 68.85 | 60.00 | 0 | 68.85 | 0 | 8.00 | 2 | True |
| S3 | 0 | beta_hours_band | 0.15 | OPTIMAL | 68.87 | 60.00 | 0 | 68.87 | 0 | 8.00 | 2 | True |
| S3 | 0 | beta_hours_band | off | OPTIMAL | 68.87 | 60.00 | 0 | 68.87 | 0 | 8.00 | 2 | True |
| S3 | 0 | Theta_night_difference | 1 | OPTIMAL | 68.80 | 60.00 | 0 | 68.80 | 0 | 8.00 | 1 | True |
| S3 | 0 | Theta_night_difference | 3 | OPTIMAL | 68.89 | 60.00 | 0 | 68.89 | 0 | 8.00 | 3 | True |
| S3 | 0 | Theta_night_difference | off | OPTIMAL | 68.89 | 60.00 | 0 | 68.89 | 0 | 8.00 | 9 | True |
| S3 | 1 | (default model) | default | FEASIBLE | 72.92 | 60.00 | 0 | 74.82 | 0 | 8.00 | 2 | True |
| S3 | 1 | G_min_rest_hours | 8 | OPTIMAL | 74.60 | 60.00 | 0 | 74.60 | 0 | 8.00 | 2 | True |
| S3 | 1 | G_min_rest_hours | 10 | FEASIBLE | 72.92 | 60.00 | 0 | 74.82 | 0 | 8.00 | 2 | True |
| S3 | 1 | G_min_rest_hours | off | OPTIMAL | 75.74 | 60.00 | 0 | 75.74 | 0 | 12.00 | 2 | True |
| S3 | 1 | beta_hours_band | 0.05 | FEASIBLE | 72.87 | 60.00 | 0 | 74.91 | 0 | 8.00 | 2 | True |
| S3 | 1 | beta_hours_band | 0.15 | FEASIBLE | 72.92 | 60.00 | 0 | 74.85 | 0 | 8.00 | 2 | True |
| S3 | 1 | beta_hours_band | off | FEASIBLE | 72.92 | 60.00 | 0 | 74.85 | 0 | 8.00 | 2 | True |
| S3 | 1 | Theta_night_difference | 1 | FEASIBLE | 72.90 | 60.00 | 0 | 74.73 | 0 | 8.00 | 1 | True |
| S3 | 1 | Theta_night_difference | 3 | OPTIMAL | 73.18 | 60.00 | 0 | 73.18 | 0 | 8.00 | 3 | True |
| S3 | 1 | Theta_night_difference | off | OPTIMAL | 73.18 | 60.00 | 0 | 73.18 | 0 | 8.00 | 11 | True |
