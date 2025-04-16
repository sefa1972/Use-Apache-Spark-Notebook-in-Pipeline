# Use-Apache-Spark-Notebook-in-Pipeline
This project aims to build a pipeline in Azure Synapse Analytics that uses an Apache Spark notebook to perform data transformation.

# Goal
By using a CSV file that contains sales order data:

  a. Transform the data using Spark

  b. Write the transformed data to a data lake in Parquet format

  c. Automate the process by embedding it into an Azure Synapse pipeline

# Technologies Used

 - Azure Synapse Analytics

 - Apache Spark

 - Azure Data Lake Storage

 - Parquet

 - CSV

 - SQL Script

# Steps

1. Run the Spark Notebook
  - The Spark Transform.ipynb file was imported.

 - Connected to the Spark pool.

 - Loaded the data from the /data folder and transformed it.

 - Saved the transformed data as Parquet in a uniquely named folder.

2. Query the Parquet Data
 - Queried the content of the created folder using SQL.

 - Confirmed that the data was successfully transformed and saved.

3. Add the Notebook to a Pipeline
 - The notebook was modified to make the folderName a parameter cell.

 - A pipeline was created with a Notebook activity added.

 - Used the system variable @pipeline().RunId as the parameter.

 - Configured the Spark pool and executor size.

4. Run and Monitor the Pipeline
 - The pipeline was published and triggered.

 - The success of the run was verified in the Monitor panel.

 - Confirmed that the Parquet files were saved in the correct folder.

# Key Learnings

 - Data transformation with Apache Spark

 - Notebook-driven data processing in Azure Synapse

 - Automating data flow using pipelines

- Parametric processing (folder naming using RunId)

👤 Author
Sefa Öztürk
IT Trainee | Azure Data Engineer in progress
📇 LinkedIn: linkedin.com/in/sefa-ozturk1972

