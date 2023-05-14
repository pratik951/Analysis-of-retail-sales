# Analysis-of-retail-sales

The code demonstrates various techniques for data analysis, data cleaning, and visualization. The steps involved in the code are explained as follows:

1)	Importing the necessary libraries such as pandas, numpy, matplotlib, seaborn, KMeans, apriori, and association_rules.
2)	Loading the dataset (online_retail_II.csv) into a pandas dataframe using pd.read_csv() function.
3)	Data Cleaning and Preparation:
•	Dropping the missing values using dropna() method.
•	Removing the negative quantity values using data[data.Quantity > 0].
•	Converting the date to datetime format using pd.to_datetime().
•	Calculating the total price using the product of the quantity and price and assigning it to a new column TotalPrice.

4)	Exploratory Data Analysis:
•	Creating a bar chart to visualize the top 10 selling products by revenue using the groupby() and agg() methods.
•	Creating a line chart to visualize the sales trend over time by category.

5)	Customer Segmentation using K-means Clustering:
•	Grouping the data by customer ID and calculating the total price and unique invoice values using the groupby() method.
•	Extracting the TotalPrice and Invoice columns and converting them to a numpy array.
•	Implementing K-means clustering algorithm with 3 clusters using the KMeans() method.
•	Assigning the cluster labels to the customers and creating a scatterplot to visualize the customer segments.

6)	Association Rule Mining:
•	Grouping the data by invoice and description and summing the quantities of the items purchased using groupby() method.
•	Unstacking the data and filling the missing values with zero.
•	Applying apriori algorithm on the basket of items with a minimum support of 0.05.
•	Applying association rules on the frequent items with a minimum threshold of 1 and sorting the rules based on their lift values.

7)	Data Visualization:
•	Displaying the charts using plt.show() method.

This code can be used as an example to analyze similar datasets and demonstrate various techniques for data analysis and visualization.
