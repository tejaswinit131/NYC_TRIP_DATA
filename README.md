# NYC_TRIP_DATA

New York Taxi Trip Data Processing
This project processes New York Taxi Trip data for the year 2019 to derive analytical insights and load the processed data into a SQLite database for further analysis.

Environment Setup
Ensure you have the following Python packages installed:

Python 3.7+
Pandas
Requests
TQDM
SQLite3
Matplotlib
Seaborn
You can install the required packages using pip:


pip install pandas requests tqdm matplotlib seaborn sqlite3

Project Structure
The project contains the following scripts:

data_extraction.py:

Extracts taxi trip data for the year 2019.
Downloads and saves parquet files from a given source.
data_processing.py:

Processes the extracted data.
Cleans and transforms the data for analysis.
Handles large datasets efficiently.
data_loading.py:

Loads the processed data into a SQLite database.
Creates necessary tables and indexes.
data_analysis.py:

Generates visualizations and insights from the processed data.
Includes charts for peak hours of taxi usage, effects of passenger count on fare, and usage trends over the year.

nyc-taxi-data-processing
Run the data extraction script:
python data_extraction.py


Run the data processing script:
python data_processing.py


Load the processed data into SQLite:
python data_loading.py


Generate visualizations:
python data_analysis.py
Data Analysis
This project includes visualizations to analyze:

Peak Hours for Taxi Usage: Identifies the hours with the highest taxi trip frequency.
Effect of Passenger Count on Trip Fare: Examines how the number of passengers affects the trip fare.
Trends in Taxi Usage Over the Year: Analyzes taxi usage trends throughout the year.







