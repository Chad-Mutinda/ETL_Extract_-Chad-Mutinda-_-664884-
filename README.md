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
  
I have included "Lab 5 Files" which contains screenshots and files of the data transformation of "sales_data_large".   
