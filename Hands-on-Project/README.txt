Assuming the data inside the a.zip was big data.  So, we using PySpark to process

Steps :
-----

01. Unzip the zipped file
02. Check emptiness of the .ack file 
03. Convert the .ack file to Spark Data Frame and read data
04. Read .dat file names and check its sanity(presence and file size)
05. Check the .dat file row count with .ack no.of records
06. If everything fine then make it as a single file
07. Save this Data Frame as table in hive by enabling hive support
08. Validate whether data saved in specified DB and Table
09. Post validating, read the same data using spark SQL
10. Atlast print the data taken from Hive using spark SQL
