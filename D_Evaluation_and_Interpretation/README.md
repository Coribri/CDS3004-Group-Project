# D — Evaluation & Interpretation of Findings

Member D: ZOU Rongbin (Richard)

This section compares Part C’s original test results with the majority-class baselines and explains the class errors and study limitations. KNN classified 6 of 10 survey test cases and 13 of 29 UCI higher-education test cases correctly. The respective baselines classified 5 and 11 correctly. In the UCI test set, KNN missed all five cases in each of two GPA bands.

The evaluation also checks four study habits individually in each sample. Attendance had the largest estimated association with GPA band in both samples. The eight adjusted comparisons were inconclusive at the 0.05 threshold. The report and notebook include the cohort-specific counts and methods.

| File | Contents |
| --- | --- |
| [Part D report](Part_D_Evaluation_and_Interpretation.docx) | English report section for the group submission |
| [Evaluation notebook](part_d_evaluation_final.ipynb) | Source checks, metric calculations and the original test outcomes |
| [KNN confusion matrices](D_KNN_Confusion_Matrices.png) | Counts by actual and predicted GPA band for both test sets |

## Run the notebook

Install `pandas`, `numpy`, `openpyxl` and `matplotlib`. Set `INPUT_DIR` in the first code cell to the folder containing the following project inputs, then run all cells.

- `survey_cleaned_python.xlsx` (the notebook also accepts `survey_cleaned_python (1).xlsx`)
- `Combined_Survey_and_UCI_Data.xlsx`
- `student_performance_cleaned.csv`
- Part C’s UCI `split.csv` and `test_predictions.csv` from the original run

The saved notebook outputs and figure display aggregate counts and metrics. Ask the group for access to the input files when reproducing the calculations. The 145-record UCI higher-education dataset supports a separate GPA model. The 1,044 Portuguese secondary-school subject records are background for Part B’s exploratory analysis.
