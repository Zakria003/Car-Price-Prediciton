

# Car Price Prediction

## Project Overview

This project focuses on predicting car prices using a dataset that includes details about car models, manufacturers, year of manufacture, price, kilometers driven, and fuel type. The dataset is preprocessed to handle missing values, invalid entries, and data type inconsistencies. This README provides an overview of the data, preprocessing steps, and the structure of the code.

## Dataset

The dataset used for this project contains information about used cars. The main features of the dataset are:

- **name**: Name of the car model
- **company**: Manufacturer of the car
- **year**: Year of manufacture
- **Price**: Price of the car (in INR)
- **kms_driven**: Distance driven by the car (in kilometers)
- **fuel_type**: Fuel type used by the car

### Sample Data

| name                          | company  | year | Price   | kms_driven | fuel_type |
|-------------------------------|----------|------|---------|------------|-----------|
| Hyundai Santro Xing XO eRLX Euro III | Hyundai  | 2007 | 80,000  | 45,000 kms | Petrol    |
| Mahindra Jeep CL550 MDI       | Mahindra | 2006 | 4,25,000 | 40 kms     | Diesel    |
| Maruti Suzuki Alto 800 Vxi    | Maruti   | 2018 | Ask For Price | 22,000 kms | Petrol    |
| Hyundai Grand i10 Magna 1.2 Kappa VTVT | Hyundai | 2014 | 3,25,000 | 28,000 kms | Petrol    |
| Ford EcoSport Titanium 1.5L TDCi | Ford | 2014 | 5,75,000 | 36,000 kms | Diesel    |

## Data Preprocessing

The dataset underwent several preprocessing steps to ensure data quality and suitability for analysis:

1. **Handling Missing Values**:
   - Removed rows with missing values in critical columns: `kms_driven` and `fuel_type`.

2. **Data Type Conversion**:
   - Converted `year` from object to integer.
   - Converted `Price` from object to integer after removing commas.
   - Converted `kms_driven` from object to integer after removing commas and extraneous text.

3. **Data Cleaning**:
   - Removed invalid entries from `year`, `Price`, and `kms_driven`.
   - Standardized `name` to include only the first three words to simplify the data.

4. **Reorganization**:
   - Reset the index after cleaning to ensure a continuous index without gaps.

## Exploratory Data Analysis (EDA)

### Data Summary

- **Number of Entries**: 816
- **Columns**: 6

#### Data Types

| Column        | Data Type |
|---------------|-----------|
| name          | object    |
| company       | object    |
| year          | int32     |
| Price         | int32     |
| kms_driven    | int32     |
| fuel_type     | object    |

### Unique Values

- **Year**: Includes valid years ranging from 2000 to 2019.
- **Price**: Converted to numeric values, now ranges from 45,000 to 28,00,000 INR.
- **Kms Driven**: Cleaned to numeric values representing kilometers driven.
- **Fuel Type**: Includes 'Petrol', 'Diesel', and 'LPG'.

## Code Usage

To run the preprocessing and EDA code, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/car-price-prediction.git
   ```

2. **Install Required Libraries**:
   Ensure you have the necessary Python libraries installed:
   ```bash
   pip install numpy pandas
   ```


## Contribution

Feel free to contribute to this project by submitting issues or pull requests. Contributions such as additional preprocessing techniques, new features, or improvements in code efficiency are welcome.


## Contact

For any questions or further information, please contact [zakriaimdad012+github@gmail.com](mailto:zakriaimdad012+github@gmail.com).

