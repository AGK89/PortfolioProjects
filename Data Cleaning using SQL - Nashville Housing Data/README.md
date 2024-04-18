# Data Cleaning in SQL Queries

![alt text]()

This repository contains SQL queries designed for cleaning and standardizing data in the `NashvilleHousing` dataset. These queries address various data cleaning tasks such as standardizing date formats, populating missing property addresses, breaking down addresses into individual columns, transforming fields, removing duplicates, and dropping unused columns. Below is an overview of each query's purpose and functionality:

## Standardize Date Format

This query standardizes the `SaleDate` column format to the date data type for consistency and ease of manipulation.

## Populate Property Address Data

Addresses with missing values are populated by matching them with corresponding addresses from different records sharing the same `ParcelID`.

## Breaking out Address into Individual Columns (Address, City, State)

The `PropertyAddress` column is split into separate columns for street address, city, and state, facilitating better analysis and organization.

## Parsing Owner Address

The `OwnerAddress` column is parsed into separate columns for address, city, and state using the `PARSENAME` function, enhancing clarity and usability.

## Change Y and N to Yes and No in "Sold as Vacant" Field

Values 'Y' and 'N' in the `SoldAsVacant` column are replaced with 'Yes' and 'No' respectively for clearer interpretation.

## Remove Duplicates

Duplicate records are identified using a common table expression (CTE) and are removed to maintain data integrity.

## Delete Unused Columns

Unused columns such as `OwnerAddress`, `TaxDistrict`, and `SaleDate` are dropped from the dataset to streamline data storage and processing.

Feel free to explore these SQL queries for cleaning and preparing your dataset for analysis or further processing. If you have any questions or suggestions for improvements, please don't hesitate to reach out. Thank you for visiting!

*Note: These queries are intended for educational and demonstration purposes. Please ensure to review and adapt them according to your specific dataset and requirements before execution.*
