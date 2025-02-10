
# Zomato Data Analysis

## Overview
This project analyzes Zomato restaurant data to clean, preprocess, and extract meaningful insights. The dataset includes various restaurant attributes such as ratings, cost for two, cuisines, and locations.

## Dataset
- Source: `zomato.csv`
- Contains information about restaurants, their ratings, cost, cuisines, and locations.

## Steps Performed
1. **Data Loading**: Read the dataset using Pandas.
2. **Data Cleaning**:
   - Dropped unnecessary columns (`url`, `dish_liked`, `phone`, `rest_type`, `reviews_list`, `menu_item`, `listed_in(type)`).
   - Renamed columns for clarity (`rate` → `rating`, `approx_cost(for two people)` → `two_people_cost`).
   - Removed duplicate entries.
   - Handled missing values (`rating` filled with mean, dropped rows with missing `location`, `cuisines`, and `two_people_cost`).
3. **Data Processing**:
   - Used SQL queries (`pandasql`) for data selection.
   - Categorized restaurant types.

## Technologies Used
- Python (Pandas, PandasSQL)
- Jupyter Notebook

## How to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/zomato-data-analysis.git
   ```
2. Navigate to the project directory:
   ```sh
   cd zomato-data-analysis
   ```
3. Install dependencies:
   ```sh
   pip install pandas pandasql jupyter
   ```
4. Run the Jupyter Notebook:
   ```sh
   jupyter notebook zomato_data_analytics.ipynb
   ```

## Future Enhancements
- Perform exploratory data analysis (EDA) and visualizations.
- Build predictive models for restaurant success based on ratings.
- Deploy a web dashboard for interactive analysis.

## Author
Sarabjeet Singh



