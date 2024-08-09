# PEI_Assessment
      A. Prerequisites
Python 3.x
Databricks Community Edition

      B. Installation
Download maven package for reading excel in spark :
Go to cluster configurations. Then go to the library tab and click Install New.
Select maven in the library source and click search packages. 
Search com.crealytics in maven dropdown in the search tab and select the version that is most suitable to your cluster configuration and spark version.
For this assessment I have selected the following version : com.crealytics:spark-excel-2.12.17-3.2.2_2.12:3.2.2_0.18.1

      C. Workflow
1. Upload the data files to dbfs in databricks.  
2. Import the necessary packages required for the entire spark project and initialise SparkContext.
3. Read order data (in json format). Correct column naming, remove invalid characters. Conduct schema and data type validation tests.
 Read customer data (in excel format). Format customer name and phone number columns to remove special characters, unnecessary spaces and numbers where not needed.
4. Read product data (in csv format). Verify states and conduct schema and data type validation tests. 
5. Save and Write the order, customer and product data frames to delta tables.
6. Create enriched tables for Q3 and Q4. Run schema and data type validation tests for the enriched tables. 
7. Run queries using spark sql for Q5 (a to d).
