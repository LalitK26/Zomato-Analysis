# Zomato Restaurant Analysis & Interactive Dashboard

A comprehensive data analysis project using the Zomato Bangalore dataset to explore restaurant trends, customer preferences, and pricing. The project includes extensive data cleaning, exploratory data analysis (EDA), and an interactive search dashboard built with Jupyter Widgets.

## 📊 Project Overview
This repository contains two primary notebooks:
1. **Analysis and Visualization**: Focuses on data preprocessing, cleaning, and extracting insights through various statistical plots.
2. **Dashboard to Search**: A practical tool that allows users to search for restaurants based on criteria like name, location, rating, and budget.

## 🛠️ Data Cleaning Steps
The raw Zomato dataset undergoes several cleaning steps to ensure accuracy and consistency:
- **Redundant Data Removal**: Dropped columns that do not contribute to analysis, such as `url`, `address`, `phone`, `menu_item`, and `reviews_list`.
- **Handling Duplicates**: Removed duplicate records to maintain dataset integrity.
- **Rating Normalization**: 
    - Handled "NEW" and "-" values as nulls.
    - Stripped the "/5" suffix and converted ratings to a standard float format.
    - Imputed missing ratings using the mean value.
- **Cost Formatting**: Converted the `approx_cost(for two people)` column from strings with commas to numeric values for quantitative analysis.
- **Categorization of 'Others'**: Grouped low-frequency rest types, locations, and cuisines into an "others" category to simplify visualizations and improve interpretability.

## 📈 Exploratory Data Analysis (EDA)
Key insights derived from the data include:
- **Location Trends**: Identifying areas with the highest density of restaurants (e.g., BTM, HSR).
- **Service Availability**: Visualizing the distribution of restaurants offering online delivery vs. those with table booking facilities.
- **Ratings Distribution**: Analyzing the spread of customer satisfaction across different restaurant types.
- **Top Chains**: Discovering which restaurant brands have the largest presence in Bangalore.
- **Price Analysis**: Understanding the average cost for two people across different locations and establishment types.

## 🖥️ Interactive Dashboard Features
The search dashboard provides a user-friendly interface to navigate the dataset:
- **Search by Name**: Instantly filter restaurants by their brand name.
- **Multi-Criteria Filter**: Find the perfect dining spot by selecting:
    - **Location**: Pick from sorted lists of major Bangalore areas.
    - **Restaurant Type**: Filter by Buffet, Cafe, Delivery, Dine-out, etc.
    - **Minimum Rating**: Set a threshold for quality.
    - **Maximum Budget**: Define your price range for a cost for two.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/LalitK26/Zomato-Analysis.git
   ```
2. Install the required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn ipywidgets
   ```
3. Open the Jupyter notebooks:
   ```bash
   jupyter notebook analysis_and_visualization.ipynb
   ```
4. To use the dashboard, ensure you have `ipywidgets` enabled in your Jupyter environment.

## 🧰 Technologies Used
- **Python**: Core programming language.
- **Pandas & NumPy**: Data manipulation and numerical operations.
- **Matplotlib & Seaborn**: Data visualization.
- **IPyWidgets**: Interactive dashboard components.

---
*Created as a deep dive into the food landscape of Bangalore.*
