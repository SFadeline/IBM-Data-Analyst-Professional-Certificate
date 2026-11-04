# IBM Data Analyst Professional Certificate

This repository is a growing collection of hands-on labs completed during the IBM Data Analyst Professional Certificate. The notebooks cover data collection and analysis using Python, APIs, web scraping, Excel, SQL, and visualization.

## Repository layout

### Data Analysis with Python

#### Accessing Data Using APIs

The Flask API lab loads job posting records from `jobs.json`. A client notebook retrieves and filters postings by technology or US location, then saves the counts in Excel workbooks.

- `Collecting_job_data_using_APIs-Lab (1).ipynb` — client notebook for requesting and analyzing job posting data.
- `Jobs_API (1).ipynb` — Flask server notebook.
- `jobs.json` — dataset used by the API.
- `job-postings.xlsx` — job counts by location.
- `job-postings-by-skill.xlsx` — job counts by technology.

#### Web Scraping

The web scraping lab retrieves a webpage and extracts programming language names and average annual salaries.

- `Web-Scraping-Lab.ipynb` — scraping notebook.
- `popular_languages.csv` — extracted language and salary data.

## Running the notebooks

Install the required packages with:

```bash
pip install flask requests pandas beautifulsoup4 openpyxl
```

For the Jobs API lab, keep the Flask server notebook running while you run the client notebook in the same Jupyter environment. The server reads `jobs.json` from its working folder.

The Web Scraping notebook retrieves the course webpage and writes the extracted data to a CSV file.

## Data sources

The job postings are from the modified dataset supplied with the course lab. The original dataset is listed on [Kaggle](https://www.kaggle.com/promptcloud/jobs-on-naukricom).

The programming language and salary table is from the [IBM lab webpage](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DA0321EN-SkillsNetwork/labs/datasets/Programming_Languages.html).

These are course datasets and do not represent live job openings or current salary estimates.
