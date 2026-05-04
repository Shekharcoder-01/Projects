# Zomato Data Cleaning & Preprocessing

## Description
This project focuses on cleaning and preparing the Kaggle Zomato Bangalore Restaurants dataset for analysis. The script processes raw data to handle missing values, remove noise, and standardize columns like ratings and costs to make the dataset ready for visualization or machine learning.

## Key Features
- **Data Cleaning**: Handled messy strings in the `rate` column (e.g., "NEW", "-") and converted them to floats.
- **Outlier Removal**: Used Z-score filtering on `votes` and `Cost2plates` to remove extreme data points.
- **Categorical Optimization**: Grouped low-frequency categories in `rest_type`, `location`, and `cuisines` into an "others" category for better grouping.
- **Text Preprocessing**: Cleaned restaurant names and review lists using Regular Expressions (Regex).
- **Data Transformation**: Renamed columns for better readability and handled null values using mean imputation and "unknown" placeholders.

## Technologies Used
- **Python 3.x**
- **Pandas**: Data manipulation and cleaning.
- **NumPy**: Numerical operations.
- **Matplotlib & Seaborn**: Data exploration.
- **SciPy**: Statistical outlier detection (Z-score).

## Project Structure
- `zomato.ipynb` (or `.py`): The main cleaning script.
- `zomato.csv`: The raw input dataset (not included in repo usually).
- `zomato2.csv`: The final cleaned output file.

## Installation & Usage
1. Clone this repository.
2. Ensure you have the `zomato.csv` file in your local path.
3. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scipy
   ```
4. Run the script:
   ```bash
   python your_script_name.py
   ```

## Dataset Note
The input file `zomato.csv` is expected to contain columns such as `address`, `rate`, `votes`, `approx_cost(for two people)`, and `rest_type`. The output `zomato2.csv` will be generated in the same directory.
# Projects
