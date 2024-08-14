# Home Sales Analysis with SparkSQL

## Table of Contents

- [Background](#background)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Setup](#setup)
- [Analysis Process](#analysis-process)
- [Results](#results)
- [Performance Optimization](#performance-optimization)
- [Conclusion](#conclusion)
- [Future Work](#future-work)

## Background

This project analyses home sales data to derive insights using Apache Spark and SparkSQL. By leveraging the distributed computing capabilities of Spark, the project aims to efficiently process and analyze large datasets, enabling more informed decision-making in the real estate market.

## Objectives

1. Calculate the average price for four-bedroom houses per year.
2. Determine the average price of homes with 3 bedrooms and 3 bathrooms based on the year they were built.
3. Analyze the average price of homes with specific features (3 bedrooms, 3 bathrooms, 2 floors, and a minimum of 2000 sqft living area).
4. Identify the average price for homes based on their "view" rating and filter those with an average price of at least $350,000.

## Dataset

The dataset used in this project is sourced from [Citi Bike Data](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv), which includes information on home sales such as price, number of bedrooms, bathrooms, living area, and more.

## Technologies Used

- **Python**: The programming language used for data processing and analysis.
- **PySpark**: Python API for Apache Spark, used for data processing and querying.
- **Google Colab**: An online interactive environment to write and execute code.
- **GitHub**: For version control and collaboration.


## Setup

To replicate this analysis, follow these steps:

1. **Clone the repository**: Clone this repository to your local machine.
   ```bash
   git clone https://github.com/yourusername/Home_Sales.git
   ```
2. **Install PySpark: Make sure PySpark is installed in your Python environment.
   ```bash
   pip install pyspark
   ```
3. Run the Jupyter Notebook: Open the Home_Sales.ipynb file in Google Colab and run the cells to execute the analysis.

## Analysis Process

The analysis is structured as follows:

- **Data Ingestion**: Reading the CSV file into a Spark DataFrame.
- **Creating a Temporary View**: Transforming the DataFrame into a Spark SQL temporary view for easier querying.
- **Executing Queries**: Running various SQL queries to extract insights based on the project's objectives.
- **Performance Optimization**: Using Spark's caching and Parquet file format to optimize the performance of the queries.

## Results

- **Average Price for Four-Bedroom Houses Per Year**: The analysis shows how the average price for four-bedroom houses has fluctuated over the years.
- **Average Price for 3 Bedroom, 3 Bathroom Homes by Year Built**: This provides insights into the value trends of these homes relative to their construction year.
- **Average Price for Homes with Specific Features**: The results indicate the average pricing trend of homes that meet certain criteria.
- **Average Price Per "View" Rating**: Homes with a higher "view" rating tend to have a higher average price, with a notable price increase for ratings with an average price above $350,000.

## Performance Optimization

Caching and Parquet format were used to improve query execution time. These optimizations demonstrated significant performance improvements, making the analysis more efficient.

## Conclusion

This project successfully demonstrates the capability of SparkSQL in handling large datasets and deriving valuable insights from home sales data. By analyzing various aspects of home prices, the project provides a comprehensive understanding of the real estate market dynamics.

## Future Work

- **Expand the Analysis**: Incorporate additional factors such as location, proximity to amenities, and historical pricing trends.
- **Predictive Modeling**: Develop machine learning models to predict future home prices based on the analyzed features.
- **Interactive Dashboard**: Create a user-friendly interface to allow real-time data analysis and visualization.
