
# NHS English Prescribing Data (EPD) Analysis Using Python and SQL  

## Overview  
This project focuses on extracting and analyzing **NHS English Prescribing Data (EPD)** from the **CKAN (Open Data Portal) API** using SQL and Python. The analysis includes data retrieval, cleaning, exploratory data analysis (EDA), and key insights into prescribing patterns across various regions and medications.  

## Dataset  
The dataset is available on the NHS Open Data Portal (CKAN):  
🔗 [English Prescribing Data (EPD) Dataset](https://opendata.nhsbsa.net/dataset/english-prescribing-data-epd)  

## Extracting Data from CKAN API Using SQL  
The NHS CKAN API provides a **Datastore API** to fetch data directly using SQL queries.  

### 1. Fetching Data Using CKAN API  
To retrieve data, use the following API endpoint:  
https://opendata.nhsbsa.net/api/3/action/datastore_search_sql?sql=<SQL_QUERY>

Replace `<SQL_QUERY>` with your SQL statement.  

### 2. Example SQL Query to Filter Data  
Fetch prescribing data for a specific **resource_id**, **BNF Chemical Substance**, and **Practice Code**:  

```sql
SELECT * 
FROM "resource_id" 
WHERE "BNF_CHEMICAL_SUBSTANCE" = 'Paracetamol' 
AND "PRACTICE_CODE" = 'A12345';

Replace "resource_id" with the actual resource ID for the EPD dataset.
Update BNF_CHEMICAL_SUBSTANCE to filter by a specific medication.
Use PRACTICE_CODE to filter by a specific GP practice.


### 3. Getting the Resource ID
To obtain the correct `resource_id`, use the API:
[https://opendata.nhsbsa.net/api/3/action/package_show?id=english-prescribing-data-epd](https://opendata.nhsbsa.net/api/3/action/package_show?id=english-prescribing-data-epd)

## Technologies Used
- 🐍 **Python**
- 📓 **Jupyter Notebook**
- 🛢️ **SQL** for data extraction
- 🔍 **CKAN API** for open data retrieval
- 📊 **Pandas** for data manipulation
- 📈 **Matplotlib & Seaborn** for visualization

