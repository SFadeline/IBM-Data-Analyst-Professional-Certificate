# Exploratory Data Analysis: Stack Overflow Developer Survey

This project uses Python to explore the Stack Overflow survey dataset from the IBM Data Analyst hands-on labs. It examines developer industries, job satisfaction, remote-work preferences, programming languages, compensation, outliers, and correlations.

## Project files

- **Exploratory_Data_Analysis.ipynb** — loads the survey data and performs the exploratory analysis.
- **Survey dataset** — loaded from the course URL when the notebook runs; the large CSV is not stored in this folder.

## Requirements

Install the Python packages with:

~~~bash
pip install pandas numpy matplotlib seaborn jupyter
~~~

## Run the project

1. Open Exploratory_Data_Analysis.ipynb in Jupyter Notebook, JupyterLab, or Google Colab.
2. Run the cells from top to bottom.
3. The notebook downloads the survey CSV from its hosted source, so an internet connection is required.

## Analysis included

- Inspect dataset structure, data types, and missing values.
- Explore industry, job-satisfaction, and remote-work distributions.
- Count programming-language responses from Malaysia.
- Compare compensation across countries and identify IQR outliers.
- Examine correlations involving experience, compensation, satisfaction, and approximate age ranges.

## Data source

[Course-provided Stack Overflow survey dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/n01PQ9pSmiRX6520flujwQ/survey-data.csv)

## Notes

The results describe survey responses, not the entire developer workforce. Compensation may be highly skewed, IQR-flagged values are not necessarily errors, and correlation does not prove causation. Numeric age values are approximations based on age ranges.
