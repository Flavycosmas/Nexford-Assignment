# Employee Salary Data Processing Assignment

## Project Overview

This project processes the San Francisco employee salary dataset using Python and R. It demonstrates data import, employee searches, dictionary-based processing, error handling, CSV export, ZIP compression, and reading exported data in R.

## Project Files

- `sf-salary.ipynb` — Jupyter Notebook containing the Python code.
- `Salaries.csv` — Original salary dataset.
- `Employee Profile/employee_details.csv` — Exported employee records.
- `Employee Profile.zip` — Compressed archive containing the exported CSV.
- `README.md` — Project documentation and execution instructions.

## Requirements

- Python 3
- Jupyter Notebook or JupyterLab
- pandas
- R

## How to Run the Python Notebook

1. Place `Salaries.csv` in the same folder as `sf-salary.ipynb`.
2. Open a terminal in the project folder.
3. Start JupyterLab by running `jupyter lab`.
4. Open `sf-salary.ipynb`.
5. Run the notebook cells in order.
6. Execute the export cell to generate `Employee Profile/employee_details.csv`.
7. Execute the ZIP creation cell to generate `Employee Profile.zip`.

## How to Run the R Code

1. Open R or the R console.
2. Set the working directory to the project folder. For example:

   `setwd("~/Documents/nexford/Employee Salary Assignment")`

3. Extract the archive:

   `unzip("Employee Profile.zip", exdir = "Employee Profile Extracted")`

4. Import the CSV:

   `employee_data <- read.csv(file.path("Employee Profile Extracted", "Employee Profile", "employee_details.csv"))`

5. Display the data:

   `head(employee_data)`

6. Check the number of records:

   `nrow(employee_data)`

## Expected Result

The R script successfully extracts the ZIP archive, imports the employee CSV file, and displays the employee records. The current exported dataset contains 148,654 records and 8 columns.

## Notes

Run the Python export and ZIP creation cells again whenever you change the exported employee records. Then rerun the R extraction and import steps to use the latest data.
