# Jobs Data Collection Using a Flask API

This project uses a Flask API and Python to explore job posting data. It counts job postings by technology and by selected US locations, then saves the results to Excel files.

## Project files

- `Jobs_API.ipynb` — loads `jobs.json` and starts the Flask API.
- `Collecting_Job_Data_Using_APIs.ipynb` — requests job data, counts postings by technology and location, and creates Excel results.
- `jobs.json` — the job posting dataset used by the API.
- `job-postings.xlsx` — job counts by location.
- `job-postings-by-skill.xlsx` — job counts by technology.

## Requirements

Install the Python packages with:

```bash
pip install flask requests pandas openpyxl
```

## Run the project

1. Put `Jobs_API.ipynb`, `Collecting_Job_Data_Using_APIs.ipynb`, and `jobs.json` in the same working folder.
2. Open `Jobs_API.ipynb` in Jupyter and run the cell that starts Flask. Keep that notebook and its kernel running.
3. Open `Collecting_Job_Data_Using_APIs.ipynb` in another notebook tab in the same Jupyter environment.
4. Run its cells to retrieve and filter the data. The notebook saves the results as Excel files.

The client notebook connects to the local API at `http://127.0.0.1:5000`.

## API endpoints

- `GET /` — displays a welcome message.
- `GET /data/all` — returns the full dataset as JSON.
- `GET /data` — searches by a supported field, such as `Location` or `Key Skills`.

For example, the client can request a location search using:

```python
requests.get(
    "http://127.0.0.1:5000/data",
    params={"Location": "New York"}
)
```

## Dataset

This lab uses a modified subset of the job posting dataset provided by the course. The original dataset is listed on [Kaggle](https://www.kaggle.com/promptcloud/jobs-on-naukricom). The data is a course dataset and does not represent live job openings.
