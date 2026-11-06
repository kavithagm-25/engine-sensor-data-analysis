# Engine Sensor Data Analysis & Performance Monitoring

## Project Overview

This project analyzes simulated turbofan engine sensor data from the NASA C-MAPSS FD001 dataset.

The goal is to understand engine performance, identify sensor trends, and detect unusual sensor readings using Python, SQL, and Power BI.

## Tools Used

- **Python:** Pandas, Matplotlib
- **SQL:** SQLite
- **Power BI:** Dashboard creation and DAX measures
- **Dataset:** NASA C-MAPSS FD001

## Project Workflow

1. Cleaned and explored sensor data from 100 engines.
2. Analyzed sensor trends and identified Sensor 11 as a useful monitoring indicator.
3. Created a reference threshold using early operating cycles.
4. Developed a simple five-consecutive-cycle rule to flag sustained sensor deviations.
5. Evaluated the rule on 20 held-out engine histories.
6. Used SQL to summarize engine performance and monitoring results.
7. Created a Power BI dashboard to visualize key findings.

## Key Findings

- Analyzed 100 simulated engine histories.
- Average engine lifetime: 206.31 operating cycles.
- Engine 69 had the longest recorded lifetime at 362 cycles.
- Sensor 11 generally increased as engines approached failure.
- The monitoring rule generated alerts for all 20 held-out engines, with an average lead time of 35.95 cycles.

**Limitation:** The monitoring results are exploratory. The dataset contains run-to-failure histories, and the evaluation does not establish real-world failure prediction accuracy or false-alarm rates.

## Dashboard

The Power BI dashboard includes:

- Total Engines
- Average Engine Lifetime
- Engine 1 Sensor 11 Trend
- Top 5 Engines by Operating Lifetime

## Skills Demonstrated

Python data analysis, data cleaning, SQL querying, exploratory analysis, sensor monitoring, DAX, and Power BI visualization.