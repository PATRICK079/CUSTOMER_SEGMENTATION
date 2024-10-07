# CUSTOMER SEGEMENTATION (KMEANS AND HIERARCHICAL)

<img width="418" alt="Screen Shot 2024-10-07 at 23 30 13" src="https://github.com/user-attachments/assets/9d011bd8-34b7-4705-be21-fee4a3ae77f1">

# Introduction

This Customer Segmentation Project aims to categorize customers into distinct groups based on their behavior and demographics to enable personalized marketing strategies. By leveraging clustering techniques, we segment customers based on key features such as spending score and age. This segmentation allows businesses to better understand their customer base, identify high-value segments, and tailor their marketing efforts to increase engagement and profitability.

The project uses a combination of data analysis and machine learning algorithms to find patterns in customer data, enabling informed decision-making for marketing, product development, and customer relationship management.


# Business Problem

The company  hired me as their machine learning engineer because they were struggling to optimize their marketing efforts due to a lack of understanding of their diverse customer base. Without clear customer segmentation, the business cannot effectively target different customer groups with tailored marketing strategies, leading to inefficient use of resources, low customer engagement, and missed opportunities for revenue growth.

The challenge is to identify distinct customer segments based on behavioral and demographic factors to enable more personalized marketing, improve customer satisfaction, and ultimately increase sales and profitability.


# Problem Encountered: Incompatible Data Type for Indexing

While working on the clustering project, I encountered an issue when attempting to index a Pandas DataFrame using boolean arrays. Specifically, the plt.scatter() function threw an error due to the boolean indexing not being compatible with the DataFrame structure. The error indicated a type mismatch between the boolean array and the DataFrame.

# Explanation of Change

To resolve this issue i had to turn the dataframe to arrays with

 data = data.values
 
 it converts it to a NumPy array using the .values attribute. This conversion ensures that boolean indexing (e.g., data[y_kmeans == 0]) is properly applied, as NumPy arrays handle boolean indexing more effectively than DataFrames in this context.

# Key Learnings from the Project

- I gained a deeper understanding of how to use clustering algorithms to segment customers based on key attributes like spending score, annual income, and age. This helped me identify distinct customer groups and tailor marketing strategies accordingly.

- I learned how to evaluate the effectiveness of different clustering methods using techniques like the Elbow Method and Dendrogram, which helped in determining the optimal number of clusters.

- I improved my ability to visualize clustering results through scatter plots and dendrograms. It was crucial for interpreting the clusters and explaining the customer segments in a clear, business-relevant manner.

- Throughout the project, I encountered challenges such as data type mismatches and clustering performance. These problems enhanced my troubleshooting skills, especially in using NumPy and Pandas to handle data correctly and ensuring that my clustering models were applied successfully.


# Model implemtation


I used both kmeans clustering and hierarchical clustering for the project

● KMeans Clustering (Spending Score & Annual Income): This provides insights into how customers with varying income levels behave in terms of spending. It helps identify high-income, high-spending customers, or lower-income groups who may still have moderate to high spending behaviors.

● Hierarchical Clustering (Spending Score & Age): This clustering reveals age-based spending habits. It might uncover generational trends, such as younger customers being more active spenders or older customers having more conservative spending patterns.


## KINDLY HAVE A LOOK AT MY DETAILED NOTEBOOK FOR INSIGHTS AND RECOMMENDATIONS. THANK YOU 
