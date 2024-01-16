
 
  Project Title: ADF ETL Pipeline that Continously Checks if a Folder is Empty in Azure Data Lake and then loads File to SQL Database Table when Folder gets Files

A.  Source Folder Details:
	 Number of Files: Initially empty and later populated with a .csv file
	 File format: CSV

B.  Target Location Details:
	 Azure SQL Database table

	

C.  Business requirements:
    Client (user) needed to check if a data lake folder is empty and then copy all files from the folder (if folder is not empty) to a table in Azure SQL Database
	

D.  Solution Steps: 
   	 -create RBAC role assignment for the storage account container 
   	 -create link services, datasets, ETL pipeline and activities
   	 -check for source folder emptiness and copy all files from the folder to the Azure SQL Database table
   	 -check the Azure SQL Database table for the copied data to confirm the pipeline runs successfully


E.  Azure Services used: 
   	 -Azure Data Lake
   	 -Azure Data Factory
   	 -Azure SQL Database
