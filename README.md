# Algorithm Analysis Project

Theoretical and experimental analysis of a probabilistic string-processing algorithm. The project derives closed-form expressions for the best, worst and average case number of basic operations, verifies them by exact counting, and compares them with measured running times.

## Contents

| Path | Description |
|---|---|
| `solution.py` | Algorithm implementation, instrumented basic-operation counters, closed-form formulas and timing experiments (standard library only) |
| `tools/brute_force_check.py` | Exhaustive verification of the average-case formula on small inputs |
| `tools/make_report_assets.py` | Generates the figures and tables used in the report |
| `report/report.tex` | Full LaTeX report with derivations and results |

## Usage

The variant of the algorithm is selected by `(No1 + No2) mod 8`.

```bash
python3 solution.py <No1> <No2>                    # timing experiment
python3 solution.py <No1> <No2> --count aabcbba    # count basic operations for a string
python3 solution.py <No1> <No2> --verify           # verify the closed-form counts
```

Developed as a two-person team project with Yigit Sarp Avci. This project was completed as part of coursework in the Computer Engineering program at Bogazici University.
