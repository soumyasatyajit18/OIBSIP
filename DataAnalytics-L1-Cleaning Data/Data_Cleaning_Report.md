# Task 3 — Data Cleaning Report

## Objective
Demonstrate a reproducible, documented data-cleaning workflow using Python, pandas, NumPy, and Jupyter Notebook.

## Dataset
A deliberately corrupted, synthetic Titanic-style passenger dataset was created for practice. It includes missing values, inconsistent categorical labels, mixed data types, currency-formatted fares, invalid category codes, implausible numeric values, sparse cabin information, and duplicate rows. It is synthetic and must not be described as authentic historical passenger data.

## Methodology
1. Audited row/column counts, null counts, dtypes, duplicates, value ranges, and category inconsistencies.
2. Normalized blank strings and whitespace.
3. Parsed numeric fields and removed currency formatting from fare.
4. Applied domain validation to age, fare, survival label, passenger class, and family-count fields.
5. Standardized `Sex` to `Male`/`Female` and `Embarked` to `S`/`C`/`Q`.
6. Removed exact duplicate records.
7. Converted sparse `Cabin` data into a `CabinKnown` indicator rather than inventing cabin values.
8. Imputed age with the median within passenger class and sex, with a global median fallback; imputed fare with passenger-class median and then global median; used mode for discrete/categorical fields; labelled missing name/ticket values as `Unknown`.
9. Used IQR fences to identify unusual numeric values. Plausible statistical outliers were retained; invalid domain values were handled as missing and imputed rather than automatically deleting records.
10. Enforced final data types, validated invariants, and exported a new CSV.

## Why outliers were not automatically deleted
IQR identifies unusual observations, not necessarily incorrect observations. High fares can be legitimate. Domain checks were therefore used to distinguish invalid values from plausible extremes, preserving useful observations and reducing avoidable bias.

## Outputs
- `Task_3_Data_Cleaning.ipynb`: complete notebook and decision justifications.
- `data/titanic_style_messy_dataset.csv`: intentionally messy input.
- `data/titanic_style_cleaned_dataset.csv`: cleaned output.
- `Cleaning_Decision_Log.csv`: decisions and rationales.
- `Before_After_Summary.csv`: high-level before/after metrics.

## Reproducibility
Run the notebook top-to-bottom from the project directory. Required libraries: `pandas` and `numpy`. The notebook writes the cleaned output to the `data` directory and runs assertions to catch remaining missing values, duplicates, invalid categories, and incorrect numeric ranges.

## Dataset sourcing note
The task brief suggests Kaggle as a source. This package uses a synthetic training dataset so the intentionally corrupted values and expected cleaning decisions are reproducible. If the evaluator requires a dataset downloaded directly from Kaggle, use the official Titanic competition dataset and preserve the original download as the unmodified source: https://www.kaggle.com/c/titanic/data
