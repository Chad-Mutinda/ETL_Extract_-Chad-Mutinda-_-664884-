# ETL Extract Lab

Chad Mutinda 
664884

## Project Description
This Jupyter Notebook ATTEMPTS to demonstrate:
- Full extraction of an entire dataset
- Incremental extraction of only new/updated records
- Timestamp tracking for incremental loads
## Tools Used
- Python 3
- pandas
- Jupyter Notebook

## How to Run
1. Install requirements: `pip install pandas jupyter`
2. Start Jupyter: `jupyter notebook`
3. Open and run `etl_extract.ipynb`

## Data Source
Sample data generated for this exercise (50+ records). "sales_data_large.csv"

## New Updates
- Added transformation logic for full and incremental datasets
- Implemented 3 transformations:
  1. Weekday extraction from dates
  2. Amount categorization (Small/Medium/Large)
  3. Discount calculation (5% for orders > $1000)

## How to Run
1. Execute cells sequentially in etl_extract.ipynb
2. Outputs will be saved as:
   - transformed_full.csv
   - transformed_incremental.csv
  
  # Lab 5 

## Lab Process Overview
Today's lab focused on the final "Load" stage of our ETL pipeline, where we took transformed data and loaded it into an optimized storage format. Here's the exact process I followed:

### Step 1: Directory Preparation
1. Created a dedicated `loaded/` directory 
2. Verified all required parent directories were present
3. Ensured proper filesystem permissions for storage operations

### Step 2: Data Loading
1. Loaded the transformed CSV files:
   - `transformed_full.csv` 
   - `transformed_incremental.csv` (new/updated records only)
2. Converted both datasets to Parquet format:
   
3. Saved outputs to:
   - `loaded/full_data.parquet`
   - `loaded/incremental_data.parquet`

### Step 3: Verification
1. Performed integrity checks by:
   - Reading back the Parquet files
   - Displaying sample records from each dataset
   - Validating record counts matched the transformed data
2. Confirmed file sizes were optimized compared to CSV

### Step 4: Documentation
1. Updated `.gitignore` to exclude binary files
2. Added clear loading instructions to README
3. Maintained complete separation between raw/transformed/loaded data

## How to Reproduce
1. **Prerequisites**:
   - Python 3.8+ with pandas and pyarrow installed

2. **Execution**:
   - Run `etl_load2.ipynb` notebook cells sequentially

3. **Expected Output**:
   - Two Parquet files in `/loaded`
   - Console confirmation of successful loading
   - Sample data preview in the notebook


