# SQL-ETL linked to GCP(Google Cloud Platform)
programming language: Python, SQL

API documentation: https://dev.socrata.com/foundry/data.cityofnewyork.us/ic3t-wcy2

dataset: url = "https://data.cityofnewyork.us/resource/ic3t-wcy2.csv"
1. Load a flat file
    writing a Python script that will load data from a flat file (a .csv-formatted text file) into
memory, and then write that data to CloudSQL database.

2. Load CSV data from an API
    use the provided API to write code that will extract
the first 100 rows of this dataset in CSV (comma-separated value) format and load them to Cloud SQL.

3. Clean data, then load data
    write code that will process ALL OF the rows of dataset(from "dataset: url" above), and clean them in
the following way, before loading them into database:
 Import only the following columns:

        ○ Job #○ Doc #
        ○ Borough
        ○ House #
        ○ Street Name
        ○ Job Type
        ○ Job Status
        ○ Job Status Descrp
        ○ Landmarked
        ○ Adult Estab
        ○ Latest Action Date
        ○ Existing Occupancy
        ○ Proposed Occupancy
        ○ Owner Type
        ○ Job Description
        ○ Initial Cost

        ● If we do not know if a record is “Landmarked”, remove it from the results. 

        ● If we do not know if a record is an “Adult Establishment,” remove it from the results. 

        ● If we do not have a “Job Description”, remove it from the results.

        ● Transform the “Initial Cost” column to be presented in tens of thousands of dollars (instead of how it is
        currently recorded, in dollars).


