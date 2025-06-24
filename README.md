# ETL_Midterm_Patricia_781
ETL pipeline for mid-semester project

## Project Overview
This project demonstrates a complete ETL (Extract, Transform, Load) pipeline for data warehousing. It processes raw data through cleaning and transformation steps before loading it into a structured format.

## ETL Phases
1. **Extract**: Loaded raw CSV files and performed initial inspection
2. **Transform**: Applied data cleaning and enrichment transformations
3. **Load**: Stored processed data in SQLite/Parquet format

## Tools Used
- Python 3
- Pandas
- SQLite3
- Jupyter Notebooks

## How to Run the Project
1. Clone the repository
2. Install requirements: `pip install pandas sqlite3 pyarrow`
3. Run notebooks in order:
   - `etl_extract.ipynb`
   - `etl_transform.ipynb`
   - `etl_load.ipynb`

