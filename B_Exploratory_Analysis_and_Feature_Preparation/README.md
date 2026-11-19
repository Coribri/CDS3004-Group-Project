# B — Exploratory Analysis & Feature Preparation

Member B: Zhau Sam Chun (4652667) · [@MyLittleHorny](https://github.com/MyLittleHorny)

Zhau Sam Chun explored 1,044 Portuguese secondary-school subject records from UCI Student Performance (dataset 320) and prepared features from the public data and the 46 university survey responses. Richard (Member D) uploaded the files on his behalf.

| File | Contents |
| --- | --- |
| [Exploratory analysis notebook](Student_Performance_EDA.ipynb) | Study time, absences and final subject grades in the UCI 320 data |
| [Feature preparation notebook](Feature_Prep_Survey_and_Public.ipynb) | Survey mappings, public-data transformations, and one-hot encoding for the exploratory table |
| [Cleaned public workbook](Student_Academic_Performance_Cleaned.xlsx) | Public subject records, data dictionary and summary |
| [Cleaned public CSV](student_performance_cleaned.csv) | The 1,044 subject records in CSV format |
| [Prepared public features](features_public_prepared.csv) | Features derived from the UCI 320 records |
| [Prepared survey features](features_survey_prepared.csv) | Public copy with five derived fields for 46 responses |
| [Combined features](features_combined.csv) | Common fields stacked from 46 survey responses and 1,044 public subject records |
| [Encoded combined features](features_combined_encoded.csv) | Same 1,090 records after one-hot encoding of study level and source |
| [Survey questionnaire](Survey_Questionnaire.md) | Blank questionnaire with original questions and options |

## Run the notebooks

Install `pandas`, `numpy`, `openpyxl`, `matplotlib` and `seaborn`. Run the EDA notebook from this folder with the cleaned workbook or CSV alongside it. To rerun feature preparation, obtain `survey_cleaned_python.xlsx` from the group and place it in the same folder as `student_performance_cleaned.csv`. The public copy of the survey feature export contains the derived fields only. Saved respondent previews have been removed from the feature preparation notebook.

## How the files relate to Parts C and D

The public data here are [UCI Student Performance (dataset 320)](https://doi.org/10.24432/C5TG7T). The two subjects are Mathematics and Portuguese, and some students appear in both. The exploratory feature table uses separate definitions of `pass` for the survey and public records. A rescaled G3 subject grade and the survey’s GPA band midpoint describe different outcomes. Part C uses the survey and [UCI Higher Education Students Performance Evaluation (dataset 856)](https://doi.org/10.24432/C51G82) for its separate classifiers. Part D evaluates those models using Part C’s original test results.
