# NYC_TRIP_DATA

New York Taxi Trip Data Processing
This project processes New York Taxi Trip data for the year 2019 to derive analytical insights and load the processed data into a SQLite database for further analysis.

Environment Setup
Firstly I Ensure that i have the following Python packages installed:

Python 3.7+
Pandas
Requests
TQDM
SQLite3
Matplotlib
Seaborn


I install the required packages using pip install


[pip install pandas requests tqdm matplotlib seaborn sqlite3]

Project Structure
The project contains the following scripts:

EXTRACTION PART:

NYC_TRIP_DATA_EXTRACTION.ipynb
I Extracted taxi trip data for the year 2019 for three months .i tried to do for a year and also for six months but i get Fatal error:[ The Python kernel is unresponsive.]
i tried to solve it i did following steps and the steps are:
1]restart cluster 
2]incresed cluster size
3]Optimize Code

I reviewed code for any inefficient operations, such as unnecessary loops, large data processing in memory, or operations that could be optimized.
used Spark's built-in functions and capabilities for distributed processing to handle large datasets more efficiently.
i extracted data for a year but i get error in processing part because of large datasets.
thus i extracted only 3 months parquet files and copied in databricks catlog .

PROCESSING PART:

NYC_TRIP_DATA_PROCESSING.ipynb

Processed the extracted data.
apllied transformation like Cleans and transforms the data for analysis.
Handles large datasets efficiently.

LOADING PART:
i write the scrips for loading processed data into a SQLite database.
also created necessary tables and indexes.

after loading part my system doesn't support.
so i only write the codes for analysis but i haven't cheaked it .
so please also consider the analysis part.


ANALYASIS PART:
NYC_TRIP_DATA_ANALYSIS.ipynb








