Exploratory Data Analysis: Stack Overflow Developer Survey

This project uses Python to explore the Stack Overflow survey dataset from the IBM Data Analyst hands-on labs. It examines developer industries, job satisfaction, remote-work preferences, programming languages, compensation, outliers, and correlations.

Project files

Exploratory_Data_Analysis.ipynb — loads the survey data and performs the exploratory analysis.

Survey dataset — loaded from the course URL when the notebook runs; the large CSV is not stored in this folder.

Requirements

Install the Python packages with:

pip install pandas numpy matplotlib seaborn jupyter

Run the project

Open Exploratory_Data_Analysis.ipynb in Jupyter Notebook, JupyterLab, or Google Colab.

Run the cells from top to bottom.

The notebook downloads the survey CSV from its hosted source, so an internet connection is required.

Analysis included

Inspect dataset structure, data types, and missing values.

Explore industry, job-satisfaction, and remote-work distributions.

Count programming-language responses from Malaysia.

Compare compensation across countries and identify IQR outliers.

Examine correlations involving experience, compensation, satisfaction, and approximate age ranges.

Data source

Course-provided Stack Overflow survey dataset

Notes

The results describe survey responses, not the entire developer workforce. Compensation may be highly skewed, IQR-flagged values are not necessarily errors, and correlation does not prove causation. Numeric age values are approximations based on age ranges.

Notes

The analysis is based on survey responses. Compensation can be highly skewed, some values are missing, and correlations show association rather than causation. Age-range correlations use approximate numeric values.
