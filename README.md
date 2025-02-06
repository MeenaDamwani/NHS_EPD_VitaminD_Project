
# NHS English Prescribing Data (EPD) Analysis Using Python and SQL  

## Overview  
This project focuses on extracting and analyzing **NHS English Prescribing Data (EPD)** from the **CKAN (Open Data Portal) API** using SQL and Python. The analysis includes data retrieval, cleaning, exploratory data analysis (EDA), and key insights into prescribing patterns across various regions and medications.  

## Dataset  
The dataset is available on the NHS Open Data Portal (CKAN):  
🔗 [English Prescribing Data (EPD) Dataset](https://opendata.nhsbsa.net/dataset/english-prescribing-data-epd)  

### **Extracting Data from CKAN API using SQL**  
The NHS CKAN API provides a **Datastore API** to fetch data directly using SQL queries.  

#### **1. Fetching Data Using CKAN API**  
To retrieve data, use the following API endpoint:  
```sh
https://opendata.nhsbsa.net/api/3/action/datastore_search_sql?sql=<SQL_QUERY>

### Technologies Used
🐍 Python
📓 Jupyter Notebook
🛢️ SQL for data extraction
🔍 CKAN API for open data retrieval
📊 Pandas for data manipulation
📈 Matplotlib & Seaborn for visualization

