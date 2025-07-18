# COVID Testing Data Collection Utility

This Python script allows users to collect and store COVID testing data, including test results, sample quality, and calibration times. It ensures the integrity of collected data by validating inputs before saving them into a CSV file.

## Features

- Collects user test data (name, result, sample quality, calibration time)
- Validates:
  - Sample quality must be above 0.9
  - Calibration time must be less than 5 minutes
- Stores valid data in a file named covid-results.csv

## How It Works

1. The user is prompted to enter:
   - Their name
   - Whether they tested positive (y) or negative (n)
   - Sample quality (float)
   - Time since last calibration (int)

2. The program checks:
   - If the sample quality is acceptable
   - If the calibration time is acceptable

3. If both checks pass, the data is stored in memory.
4. When the user types "stop", the session ends and results are saved to covid-results.csv.

##  Output

The script creates a covid-results.csv file with the following format:
name,test_result,sample_quality,calibration_time


