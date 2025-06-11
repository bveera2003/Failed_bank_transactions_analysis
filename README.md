# Failed_bank_transactions_analysis
Project Overview:
This project focuses on analyzing failed banking transactions across multiple branches of the State Bank of India in three major cities: Hyderabad, Bangalore, and Mumbai. It aims to identify patterns, potential causes, and high-failure branches using data engineering and analytics techniques.

Objectives:
	-Collect and process transaction data from multiple branches.
	-Clean and transform the data using PySpark on Dataproc.
	-Filter out failed transactions.
	-Store clean and failed data in Cloud SQL (MySQL).
	-Perform visual analysis using BigQuery and Looker Studio/Data Studio.

 Architecture
    Google Cloud Services Used:
	-Cloud Storage: Storing raw and processed CSV files.
	-Dataproc (PySpark): Data cleaning and transformation.
	-Cloud SQL (MySQL): Store filtered failed transactions.
	-BigQuery: Perform analysis and build reports.
	-Looker Studio: Visualization and dashboards.

    Technologies Used:
	-Python, PySpark
	-Google Cloud Platform
	-Cloud Storage
	-Dataproc
	-Cloud SQL (MySQL)
	-BigQuery
	-Looker Studio
	-SQL, Pandas

     How to Run:
	-Upload your branch-wise data to GCS
	-Ensure naming format is like: HYD-Ameerpet_2025-06-01.csv
	-Run PySpark cleaning job on Dataproc
	-Run filtering script to extract failed transactions
	-Insert failed data into Cloud SQL
	-Query in BigQuery and create visualizations

     Key Insights:
	-Identify top 3 branches with the highest failure rate.
	-Spot peak hours/days for failed transactions.
	-Highlight failure-prone transaction types (e.g., UPI, NEFT).
	-Detect patterns related to fraud flags.

     Future Enhancements:
	-Integrate real-time monitoring with Pub/Sub & Dataflow.
	-Alert system for abnormal failure spikes.
	-Include root cause tagging for each failure.
