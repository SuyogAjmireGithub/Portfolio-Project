# Nashville Housing Data Cleaning Project

## Description

This project focuses on cleaning and transforming housing data from the Nashville area using SQL queries. The dataset, stored in the `NashvilleHousing` table within the `PortfolioProject.dbo` schema, contains information such as property addresses, sale dates, sale prices, and more.

The data cleaning process involves several steps to standardize formats, populate missing values, split addresses into individual components, convert binary values, remove duplicates, and optimize the schema by removing unused columns.

## Key Features

- Standardize Date Format**: Ensures consistency in the representation of sale dates.
- Populate Property Address Data**: Fills in missing property addresses based on available information.
- Split Address into Individual Columns**: Separates address components (e.g., street, city, state) for better analysis.
- Convert Binary Values**: Changes 'Y' and 'N' values to 'Yes' and 'No' for readability.
- Remove Duplicates**: Identifies and eliminates duplicate records based on specific criteria.
- Delete Unused Columns**: Optimizes the schema by removing columns that are no longer needed.

