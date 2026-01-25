# Chicago Temperature Analysis (1940-2020)

Python-based statistical analysis of 80 years of temperature data from Chicago, Illinois.

## Overview

This project analyzes long-term climate trends using hourly temperature measurements from the Open-Metro API. The analysis reveals significant temperature shifts over eight decades.

## Features

- Automated data retrieval from Open-Metro API
- SQLite database storage (Chicago_temp.db)
- Statistical calculations (min, max, mean, standard deviation)
- Annual and decade-level aggregations
- Data visualization with line graphs
- CSV export functionality

This executes three modules in sequence:
1. `model_builder.py` - Downloads and stores temperature data
2. `control_data.py` - Calculates statistical measures
3. `view_data.py` - Generates visualizations

## Key Findings

Analysis of 80 years of data (1940-2020) shows:

- Average temperature increased by 1°C (2°F)
- Maximum temperature increased by 1°C (2°F)
- Minimum temperature decreased by 5°C (10°F)

| Decade | Max   | Mean  | Min     | Std Dev |
|--------|-------|-------|---------|---------|
| 1940   | 35.5  | 9.2   | -27.0   | 11.6    |
| 1950   | 36.1  | 10.0  | -26.4   | 11.5    |
| 1960   | 36.2  | 9.4   | -28.8   | 11.8    |
| 1970   | 35.4  | 9.5   | -26.5   | 11.8    |
| 1980   | 37.0  | 9.8   | -31.8   | 11.7    |
| 1990   | 37.4  | 10.3  | -32.5   | 11.0    |
| 2000   | 36.7  | 10.4  | -28.0   | 11.3    |
| 2010   | 36.9  | 10.2  | -32.4   | 11.3    |

*All temperatures in Celsius*

## Technologies

- Python 3.x
- SQLite
- Open-Metro API
- Data visualization libraries (matplotlib/seaborn)

## Project Structure
```
.
├── main.py              # Main execution script
├── model_builder.py     # Data retrieval and storage
├── control_data.py      # Statistical analysis
├── view_data.py         # Visualization generation
└── Chicago_temp.db      # SQLite database (generated)
```

## Author

Steve Eckardt  
Professional Software Development Bootcamp, Open Avenues Foundation  
October 2023 - December 2023
