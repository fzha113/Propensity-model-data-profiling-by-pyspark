# Propensity-model-data-profiling-by-pyspark

## Profile description
+ create-model-report-Dec2019.py --> Generating data quality assessment report(entry program)
+ DBconnection.py      --> building connection to EDW DB
+ conn.yaml            --> DB connection configuration file(loaded by DBconnection.py)
+ loadYaml.yaml        --> Storing SQL queries for extracting data from EDW DB
+ assess_data_quality.py  --> The main program for data processing

## Main Function description
### DataDescription
Check that the columns of the two matching tables are the same or not
### col_missing
The persentage of missing value(0, None and blank) in each columns
### row_missing
the number of missing value in each row(0, None and blank) more than half are missing
### levels
checking how many levels in each columns
### outilers
checking the 5% maxium and minium values in each columns
### correlations
calculating the correlation coefficient between each columns
