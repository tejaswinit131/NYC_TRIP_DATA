NYC Trip Data
Project Overview
This project processes New York Taxi Trip data for the year 2019 to derive analytical insights and load the processed data into a SQLite database for further analysis.

Environment Setup
Ensure the following Python packages are installed:

Python 3.7+
Pandas
Requests
TQDM
SQLite3
Matplotlib
Seaborn
Install the required packages using:

bash
Copy code
pip install pandas requests tqdm matplotlib seaborn
Project Structure
The project contains the following scripts:

Extraction Part
NYC_TRIP_DATA_EXTRACTION.ipynb

I extracted taxi trip data for three months in 2019. Attempting to process data for the entire year or six months resulted in a fatal error: "The Python kernel is unresponsive." To address this, I:

Restarted the cluster.
Increased cluster size.
Optimized the code.
I reviewed the code for inefficient operations, such as unnecessary loops or large data processing in memory, and utilized Spark's built-in functions for distributed processing.

Finally, I extracted data for three months and copied the parquet files into the Databricks catalog.

Processing Part
NYC_TRIP_DATA_PROCESSING.ipynb

After extracting the parquet files, I checked their schemas using df.printSchema(). The "For-Hire Vehicle Trip Records" files lacked the required columns, so I skipped these files and applied transformations to the remaining ones.

Transformations included:

Cleaning and transforming the data for analysis.
Removing trips with missing or corrupt data.
Deriving new columns such as trip duration and average speed.
Aggregating data to calculate total trips and average fare per day.
I displayed five records of each transformed DataFrame.

Loading Part
I wrote scripts to load processed data into a SQLite database, creating necessary tables and indexes.

Due to system limitations, I couldn't execute the analysis. I wrote the analysis code but haven't checked it.

Analysis Part
NYC_TRIP_DATA_ANALYSIS.ipynb

The analysis script is included but untested due to the system's performance issues.
