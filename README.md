# Solar_ETL

Performing Extract, Transform, and Load process on data.

Data sources: EIA solar energy and power plant CSVs, Historial NOAA weather data CSVs, US cities database CSV.

Process: 
-Read in all the CSVs to Jupyter Notebook in order to modify with Pandas.
-Modified new dataframes as needed to clean up the columns and format them correctly.
-Merged the cities, plants, and solar plants in order to get individual locations.
-In order to get the closest sunshine/city NOAA data to each plant, coverted coordinates to radians, elimiated for null values, used the haversine formula in order to get closest coordinate match up.
-Merged final tables for closest values in order to get best match in locations for annual sunshine.
-Created a new database within Postgres, with associated table, in order to load the dataframe into the database.
-Tested with SQL code in order to make sure the load was successful.