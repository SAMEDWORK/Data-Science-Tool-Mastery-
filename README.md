## Project Summary
This project demonstrates the core data science toolchain on the cleaned Breast Cancer Wisconsin (Diagnostic) dataset (569 cases, 8 tumor measurements). It combines Python, Pandas, and NumPy for analysis, Matplotlib and Seaborn for visualization, Scikit-learn for machine learning, and SQL (SQLite) for structured queries. The dataset is also exported for Power BI, and the whole workflow is documented in a Jupyter Notebook and a written report.

## Key Findings
- **Model performance:** a Logistic Regression classifier (standardized features, 80/20 stratified split) reached 92.98% accuracy, 88.64% precision, and 92.86% recall on malignant cases, with 3 missed malignant cases out of 42 in the test set.
- **Top predictors:** radius, area, texture, and perimeter have the largest standardized coefficients, so tumor size is the dominant signal.
- **SQL insight:** malignancy rate rises steadily with tumor size category, from 3.5% (Small) to 20.0% (Medium), 85.2% (Large), and 100% (Very Large).
- **Power BI:** the dataset is exported as a CSV, and the report includes a dashboard layout (KPI cards, bar and scatter charts, slicers) to build in Power BI Desktop. The dashboard itself is a specification, not a built file.

**Conclusion:** tumor size is the strongest, most interpretable predictor of malignancy, and a simple, interpretable model captures most of the signal.
