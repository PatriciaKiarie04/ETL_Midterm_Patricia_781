# ETL_Midterm_Patricia_781
ETL pipeline for mid-semester project

# ETL Pipeline Project - DSA2040A Midterm Exam

## Project Overview
This project implements a complete ETL (Extract, Transform, Load) pipeline that demonstrates fundamental data warehousing concepts. The pipeline:

1. Extracts raw data from CSV files
2. Transforms the data through cleaning, enrichment, and restructuring
3. Loads the processed data into structured formats suitable for analysis


## ETL Phases Detailed Explanation

### 1. Extract Phase (`etl_extract.ipynb`)
The extraction process involves:
- Loading source data from `raw_data.csv` and `incremental_data.csv`
- Performing initial data inspection using:
  - `.head()` to show sample records
  - `.info()` to display data structure and types
  - Basic statistics with `.describe()`
- Identifying data quality issues:
  - Missing values
  - Inconsistent formatting
  - Potential outliers
  - Data type mismatches
- Saving raw copies to preserve original data

### 2. Transform Phase (`etl_transform.ipynb`)
The transformation stage applies several data quality improvements:

1. **Missing Value Treatment**
   - Numeric columns: Filled with median values
   - Categorical columns: Filled with mode values
   - Documentation of missing value counts before/after

2. **Duplicate Removal**
   - Identified and removed exact duplicate records
   - Implemented based on business key columns

3. **Data Enrichment**
   - Created calculated fields (e.g., `total_price = quantity * unit_price`)
   - Derived new metrics from existing columns

4. **Data Type Conversion**
   - Converted string dates to proper datetime objects
   - Fixed numeric fields stored as strings
   - Standardized categorical values

5. **Structural Changes**
   - Renamed columns for consistency
   - Reordered columns for better readability
   - Split/merged columns as needed

### 3. Load Phase (`etl_load.ipynb`)
The loading stage persists the processed data in analysis-ready formats:

**Parquet Option:**
- Stored in columnar format for efficient analytics
- Preserved data types and schema
- Enabled efficient compression
- Ideal for big data processing frameworks

## Tools and Technologies Used

### Core Technologies
- **Python 3**: Primary implementation language
- **Pandas**: Data manipulation and transformation
- **Jupyter Notebooks**: Interactive development environment

### Data Storage Options
- **Parquet**: Columnar storage format (via PyArrow)

### Supporting Libraries
- **NumPy**: Numerical operations
- **Matplotlib**: Basic visualizations (for bonus)
- **datetime**: Date/time handling

## How to Run the Project

### Prerequisites
- Python 3.8+
- Jupyter Lab/Notebook
- Required packages (install via `pip install -r requirements.txt`)

### Execution Steps
1. **Clone the repository**
   
2. **Install dependencies**
  Pandas
  Parquet
  Matplotlib

3. **Run Notebooks**

4. **Verify output**

