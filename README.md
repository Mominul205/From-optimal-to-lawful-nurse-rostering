# From optimal to lawful nurse rostering: data and results

This repository contains the data and the results of the paper **"From optimal to lawful nurse rostering: a
working-time-compliant multi-objective model and a comparison of exact, hybrid and learning-based methods"** by
Mominul Islam, Md. Mushiur Rahman and Md. Limonur Rahman Lingkon (Department of Industrial and Production
Engineering, Rajshahi University of Engineering and Technology, Rajshahi 6204, Bangladesh). It holds the benchmark
data, the generated instances and every run of the experiments with its rosters.

## 1. Contents

| Folder or file | Contents | Paper |
|---|---|---|
| `data/raw/WLB` | copy of the benchmark data of Gülmez et al. (2026): result files, Excel reports and revision files (see Section 4) | Section 5.1 |
| `data/processed` | benchmark scenarios S1, S2 and S3 as instance files, the 36 published rosters and the published objective values, built from `data/raw/WLB` | Section 5.1, Table 1 |
| `data/reference` | values transcribed from the tables of Gülmez et al. (2026), used to check the processed data | Section 5.1 |
| `data/tuning` | generated instances T1 and T2 (tuning) and A1 and A2 (study of the components), with their bounds and starting rosters | Sections 5.2 and 5.6, Appendix B |
| `data/scalability` | the 15 generated instances L30-S1 to L200-S3, with their bounds and starting rosters | Section 5.4, Appendix B |
| `results/step1_data_consistency.txt` | consistency checks of the benchmark data | Section 5.1 |
| `results/validation` | measures, staff values and rule violations of the 36 published rosters, their agreement with the result files and tables of Gülmez et al. (2026), and the hypervolume of the published fronts | Sections 5.1 and 5.3.2, Table 4 |
| `results/phase3/step10` | tuning runs | Section 5.2, Appendix C |
| `results/phase5/test1` | Test 1: the five methods on the baseline formulation | Sections 5.3.1 and 5.7, Tables 3 and 8 |
| `results/phase5/test2b` | Test 2: the five methods on the proposed model, on a common grid | Sections 5.3.2, 5.3.3 and 5.7, Tables 4, 5 and 8 |
| `results/phase5/extra_solves` | four CP-SAT solves of the proposed model in exact staffing at the $F_2$ of the baseline rosters | Section 5.3.2, Figure 1 |
| `results/phase5/scalability` | scalability study | Sections 5.4 and 5.7, Tables 6 and 8, Figure 2 |
| `results/phase5/sensitivity` | sensitivity analysis | Section 5.5, Table 7, Figure 3 |
| `results/phase5/ablation` | study of the components of RL-ALNS+CP-SAT | Sections 5.6 and 5.7, Figure 4, Appendix D |

## 2. Names used in the files

| Name | Meaning |
|---|---|
| `S1`, `S2`, `S3` | benchmark scenarios; in generated instances, the pattern taken from that scenario |
| `MEDIUM`, `HARD`, `EXTREME` | fairness levels of the baseline formulation ($\theta_{\varphi}$ = 0.25, 0.15 and 0.05) |
| `TOL0`, `TOL1` | exact staffing ($\tau = 0$) and flexible staffing ($\tau = 1$) |
| `GA`, `NSGA3`, `CPSAT`, `ALNS_NO_LEARNING`, `OURS` | GA, NSGA-III, CP-SAT, ALNS+CP-SAT and RL-ALNS+CP-SAT |
| `run01` to `run30` | independent runs; the random seed equals the run number |
| `_1`, `_2`, ... at the end of a roster file | grid point of the ε-constraint procedure |
| `L30_S1` to `L200_S3` | scalability instances: number of staff members and pattern |
| `T1`, `T2`, `A1`, `A2` | generated instances for tuning and for the study of the components |

## 3. Files of an experiment

| Folder or file | Contents |
|---|---|
| `runs/` | one JSON file per run: settings of the run, objective values and feasibility of every roster found, hypervolume and time |
| `rosters/` | every feasible final roster as a CSV file with one row per assignment (staff member, day, shift) |
| `per_staff/` | for every roster, the measures of each staff member (satisfaction, hours, rests, night shifts and others) |
| `histories/` | search history of the hybrid methods: one row per destroy-and-repair iteration (time, operator, freed cells, reward, current and best $F_1$, search state) |
| `grids/` (Test 2) | grid of the ε-constraint procedure and the corner rosters of each configuration |
| `starts/` (study of the components) | common starting rosters |
| `*_runs.csv`, `*_summary.csv`, `*_statistics.csv`, `*_report.md` | summaries of the runs |
| `repair_report_*` (Test 1) | runs of ALNS+CP-SAT and RL-ALNS+CP-SAT that found no starting roster in time at a grid point, and so produced fewer front points than CP-SAT, repeated with new random seeds or more time for the starting roster |

The table numbers inside the files `test1_report.md` and `test2b_report.md` follow an earlier numbering of the
tables. The table numbers of the paper are those given in Section 1.

The instance files in `data/processed/S1` (and in every generated instance folder) are `staff.csv` (weekly
contracts and numbers of requests), `shifts.csv`, `requirements.csv` (requirement of every slot), `requests.csv`
(requested slots), `requests_matrix.csv`, `parameters.json` (rule parameters) and `derived_sets.json` (the sets of
24-hour windows, short-rest pairs and duty chains).

## 4. Benchmark data of Gülmez et al. (2026)

`data/raw/WLB` is a copy of the data files of the repository https://github.com/e-gulmez/WLB at commit
`21c14f288afcb30868cd39a80d92a87f8245bea0` (Gülmez, 2026). These files are the work of Gülmez et al. (2026), are
included unchanged so that `data/processed` can be traced to its source, and are not covered by the licence of
Section 6. Please cite:

Gülmez, E., Aydin, M. E., Urganci, K. B., Gamoura, S. C., & Koruca, H. I. (2026). Healthcare staff scheduling with
work-life balance constraint using multi objective evolutionary algorithms. *Computers & Industrial Engineering, 220*,
Article 112287. https://doi.org/10.1016/j.cie.2026.112287

## 5. Rule labels in the validation files

The rule labels in `results/validation/violations_published.csv` follow an earlier numbering of the equations. The
table gives the corresponding equations of the paper.

| Label | Rule | Equation in the paper |
|---|---|---|
| (3) | hours in any 24-hour period | (7) |
| (11) | minimum rest | (8) |
| (12) | longest continuous duty | (9) |
| (14) | working days in seven consecutive days | (10) and (11) |
| (17) | difference in unwanted shifts | (15) |
| (19) | share of contracted hours | (16) |
| (21) | difference in night shifts | (17) |
| (27) | range of the satisfaction rates (baseline formulation) | (33) |

## 6. Licence

The data and results produced in this study are released under the Creative Commons Attribution 4.0 International
Licence (CC BY 4.0), as stated in `LICENSE.md`. The files in `data/raw/WLB` are excluded (Section 4).
