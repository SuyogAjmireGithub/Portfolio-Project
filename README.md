# Nashville Housing Data Cleaning Project

This project focuses on cleaning and transforming data related to Nashville housing in a SQL Server database. The script addresses various data quality issues, such as date formatting, populating missing values, splitting addresses, transforming boolean values, removing duplicates, and dropping unused columns.

## Table of Contents

- [Overview](#overview)
- [Usage](#usage)
- [Data Cleaning Steps](#data-cleaning-steps)
- [Importing Data (Optional)](#importing-data-optional)

## Overview

The script is designed to be executed within a SQL Server environment and is tailored to the specific structure of the `NashvilleHousing` table in the `PortfolioProject` database. It is essential to understand the structure of the data and review the script thoroughly before execution.

## Usage

1. **Backup Data:**
   Before executing the script, it is recommended to create a backup of the existing data or work with a copy of the dataset to avoid unintentional data loss.

2. **Execute the Script:**
   Copy and paste the SQL script into your SQL Server Management Studio or equivalent tool. Execute the script against the `NashvilleHousing` table in the `PortfolioProject` database.

3. **Review Results:**
   After execution, review the data in the `NashvilleHousing` table to ensure that the desired data cleaning and transformation steps have been applied successfully.

## Data Cleaning Steps

### Standardize Date Format
- Converts the `SaleDate` column to a standardized date format.

### Populate Property Address Data
- Fills in missing `PropertyAddress` values by copying from another record with the same `ParcelID`.

### Split Address into Individual Columns
- Separates the `PropertyAddress` into separate columns for `Address` and `City`.

### Split Owner Address into Individual Columns
- Separates the `OwnerAddress` into separate columns for `Address`, `City`, and `State`.

### Change 'Y' and 'N' to 'Yes' and 'No'
- Updates the values in the `SoldAsVacant` column, replacing 'Y' with 'Yes' and 'N' with 'No'.

### Remove Duplicates
- Identifies and removes duplicate records based on certain columns.

### Delete Unused Columns
- Drops unused columns such as `OwnerAddress`, `TaxDistrict`, `PropertyAddress`, and `SaleDate`.

## Importing Data (Optional)

The script includes sections for importing data using `OPENROWSET` and `BULK INSERT`. These sections are currently commented out and can be used for importing data from an external source.



