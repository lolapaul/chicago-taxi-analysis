#  Chicago Taxi Analysis

Exploratory data analysis and hypothesis testing for a new ride-sharing company operating in Chicago. This project investigates passenger behavior, trip patterns, taxi company performance, and weather effects on travel durations using real-world data from November 2017.

---

##  Objective

The goal of this project is to:

- Analyze taxi usage patterns in Chicago
- Identify leading taxi companies by trip volume
- Assess demand in different city neighborhoods
- Understand the impact of weather on trip duration
- Test the hypothesis that rain affects trip time from Loop to O’Hare on Saturdays

---

##  Dataset Description

The analysis uses a database composed of four primary tables and additional CSV files:

### SQL Tables
- `neighborhoods` — Neighborhood names and IDs  
- `cabs` — Cab IDs and associated companies  
- `trips` — Trip data (timestamps, locations, duration, distance)  
- `weather_records` — Hourly weather observations with temperature and descriptions  

### CSV Files
- `project_sql_result_01.csv` — Trips by company on Nov 15–16, 2017  
- `project_sql_result_04.csv` — Average trips per neighborhood in Nov 2017  
- `project_sql_result_07.csv` — Loop to O’Hare trip durations with weather data  

---

##  Project Workflow

1. **Data Extraction & SQL Queries**
   - Identify top companies and daily usage patterns
   - Classify weather conditions and join weather with trip data

2. **Python Data Analysis**
   - Import and explore CSV results
   - Plot taxi company popularity and top drop-off neighborhoods
   - Examine distribution of trip durations and assess impact of weather

3. **Hypothesis Testing**
   - Null Hypothesis: Average trip duration on rainy Saturdays from Loop to O’Hare equals that on non-rainy Saturdays
   - Statistical test performed using SciPy

---

##  Key Questions Answered

- Which taxi companies are most active?
- What are the most popular drop-off neighborhoods?
- Does rainy weather increase trip duration to the airport?
- What insights can guide Zuber’s marketing and operational decisions?

---

##  Project Structure
```
chicago-taxi-analysis/
│
├── chicago_taxi_analysis.ipynb
├── data_extraction_script.txt
├── project_sql_result_01.csv
├── project_sql_result_04.csv
├── project_sql_result_07.csv
├── requirements.txt
└── README.md
```

---

##  Data Extraction

Prior to the Python analysis, relevant datasets were generated using SQL queries and additional data was scraped from the web.

- 🔹 `data_extraction_script.txt`: This file contains the full SQL code used to query the `trips`, `weather_records`, `cabs`, and `neighborhoods` tables to extract insights such as trip counts by company and weather conditions. It also includes Python code used to scrape historical weather data from [this external source](https://practicum-content.s3.us-west-1.amazonaws.com/data-analyst-eng/moved_chicago_weather_2017.html).

These queries and scripts formed the basis for the CSV files analyzed in the notebook.

---

##  Tools & Libraries Used

- SQL
- Python
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- Jupyter Notebook

---

##  Status

✔️ Project completed as part of the **TripleTen Bootcamp** – Sprint: *SQL & Data Interpretation*

---

##  Author

David Villanueva  
[LinkedIn](https://www.linkedin.com/in/david-villanueva-59659727)  
[GitHub](https://github.com/lolapaul)
