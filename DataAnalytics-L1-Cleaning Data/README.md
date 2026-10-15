# Task 3 — Data Cleaning Project

## Contents
- `Task_3_Data_Cleaning.ipynb` — step-by-step notebook with markdown decision justifications, audit, cleaning, IQR review, validation, and export.
- `data/titanic_style_messy_dataset.csv` — intentionally corrupted input dataset.
- `data/titanic_style_cleaned_dataset.csv` — cleaned output.
- `Cleaning_Decision_Log.csv` — concise record of cleaning decisions.
- `Before_After_Summary.csv` — key before/after metrics.



## Run
1. Open `Task_3_Data_Cleaning.ipynb` in Jupyter Notebook or JupyterLab.
2. Ensure pandas and numpy are installed: `pip install pandas numpy`.
3. Run cells from top to bottom.
4. Keep the `data` folder in the same project directory so relative paths work.

## Cleaning outcome
- Input rows: 512
- Output rows: 500
- Exact duplicate rows detected in raw input: 12
- Exact duplicate rows remaining: 0
- Missing cells remaining: 0
- Final output columns: 12

All output metrics above are generated from the files produced in this run.
