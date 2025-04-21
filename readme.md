# PyCSVDataCleaner

[![PyPI](https://img.shields.io/pypi/v/PyCSVDataCleaner)](https://pypi.org/project/PyCSVDataCleaner/)
[![Python Version](https://img.shields.io/pypi/pyversions/PyCSVDataCleaner)](https://pypi.org/project/PyCSVDataCleaner/)


**PyCSVDataCleaner** is a simple Python package designed to clean CSV files. It helps you preprocess your data by:
- Removing duplicate rows
- Removing rows with missing values
- Removing constant columns

The package is easy to use and works with CSV files containing any kind of data. It is ideal for automating the data cleaning process during your machine learning or data analysis workflow.

---

## Features

- **Remove Duplicate Rows**: Automatically removes duplicate rows from the dataset.
- **Remove Rows with Missing Values**: Cleans your dataset by eliminating rows with empty cells.
- **Remove Constant Columns**: Removes columns that contain constant values across all rows.

## Installation

You can install **PyCSVDataCleaner** via pip:

```bash
pip install PyCSVDataCleaner
```

## Usage

```bash
from PyCSVDataCleaner import PyCSVDataCleaner

input_file = 'path_to_your_input_file.csv'

output_file = 'path_to_your_output_file.csv'

PyCSVDataCleaner(input_file, output_file)
```

## Example Output
When running the script, you'll get output in the terminal indicating how many rows and columns were removed or cleaned:

```bash
Cleaning file: fine_name.csv

--- Initial Data Info ---
Rows (excluding header): 129971
Columns: 14
Removed 0 duplicate rows.
Removed 107584 rows with missing values.
Removed 1 constant columns.

--- Cleaning Done ---
Final Rows: 22387
Final Columns: 13
```
