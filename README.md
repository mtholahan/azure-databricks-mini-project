# Azure DataBricks Mini Project


## 📖 Abstract
This project demonstrates how to use Azure Databricks and PySpark to explore and transform financial transaction data. The provided lab notebook (banking_lab.dbc) contained a series of prompts guiding the construction of PySpark DataFrame operations to query, filter, and aggregate customer banking data.

Within Databricks, I imported the notebook into my workspace and iteratively implemented PySpark solutions to answer questions such as filtering transactions by type, grouping by account attributes, and aggregating customer activity. The emphasis was on applying PySpark DataFrame APIs rather than SparkSQL, building fluency with Spark’s Pythonic interface.

The exercise culminated in a completed Databricks notebook that illustrates core data engineering skills: data ingestion, transformation, aggregation, and query design in PySpark. Along the way, I deepened my understanding of PySpark syntax, DataFrame query patterns, and Databricks’ cloud-native development environment.

This project highlights how Spark-based data engineering is performed in the cloud, bridging Python workflows with distributed compute in Azure Databricks.



## 🛠 Requirements
- Azure account with Databricks workspace provisioned
- Databricks Community Edition or paid subscription
- Banking_lab.dbc file (provided project file)
- Installed locally (for testing outside Databricks):
  - pyspark >= 3.3.0
  - ipython
  - jupyter
  - pandas



## 🧰 Setup
- Log into Azure Databricks workspace
- Navigate to your user directory → Import → Upload file
- Import banking_lab.dbc into your workspace
- Open the imported notebook in Databricks



## 📊 Dataset
- Banking_lab.dbc contains sample banking data for analysis
- Structured to allow PySpark DataFrame operations and queries
- No external CSVs or APIs required; dataset bundled within .dbc archive



## ⏱️ Run Steps
- Open the imported notebook in Databricks
- Fill in Python and PySpark code where # TODO comments are indicated
- Execute cells sequentially to complete all analysis prompts
- Save completed notebook and export as .dbc for submission



## 📈 Outputs
- Completed Databricks notebook with PySpark code
- Results of DataFrame transformations and queries
- Exported .dbc file for submission



## 📸 Evidence

![databricks_notebook.png](./evidence/databricks_notebook.png)  
Screenshot of Databricks notebook in workspace

![cluster_ui.png](./evidence/cluster_ui.png)  
Screenshot of cluster configuration




## 📎 Deliverables

- [`- Databricks notebooks (.dbc export) in /deliverables/`](./deliverables/- Databricks notebooks (.dbc export) in /deliverables/)

- [`- requirements.txt`](./deliverables/- requirements.txt)

- [`- README with instructions`](./deliverables/- README with instructions)




## 🛠️ Architecture
- Azure Databricks environment hosting PySpark notebooks
- Cluster-based execution of Spark DataFrame queries
- Local dependencies only required for optional testing



## 🔍 Monitoring
- Databricks job UI shows execution status
- Spark UI available for performance inspection of transformations



## ♻️ Cleanup
- Remove imported notebook from Databricks if no longer needed
- Shut down or delete Databricks cluster to avoid unnecessary charges



*Generated automatically via Python + Jinja2 + SQL Server table `tblMiniProjectProgress` on 09-15-2025 18:04:02*