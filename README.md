# CryptoCurrencies Overview
  In this analysis we created a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. We began by preprocessing the dataset in order to perform Principal Component Analysis (PCA) later on in the analysis.

# Deliverable 1
  In the first deliverable we began by keeping all the cryptocurrencies that are being traded. We then dropped the trading columnn and removed any rows that had at least one nnull value. We then filtered the data to only hold cryptocurrencies that have been mined and followed that up by using the get_dummies() method to create variables for two text features and storing the data in a new Dataframe. 
  
 <img width="463" alt="Screen Shot 2023-04-03 at 3 59 42 PM" src="https://user-images.githubusercontent.com/117120227/229644642-9ce6c63c-fa47-478e-a218-d3eda70e0482.png">

 # Deliverable 2
  In the second Deliverable we reduced the data to three dimensions using PCA. Once reduced we created a new dataframe with columns, PC 1, PC 2, and PC 3, all while using the same index as the DataFrame created in deliverable 1. 
  
<img width="178" alt="Screen Shot 2023-04-03 at 3 59 23 PM" src="https://user-images.githubusercontent.com/117120227/229644613-f45d5c96-1802-4a7f-b776-77acd5eaf8bb.png">

# Deliverable 3
  In the third Deliverable we clustered Cryptocurrencies using K-means, then create dan elbow curve using hvPlot to find the best value for K from the DataFrame created in Deliverable 2. Then, we run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.
  
  <img width="452" alt="Screen Shot 2023-04-03 at 4 09 09 PM" src="https://user-images.githubusercontent.com/117120227/229645855-4ba4e47b-7aa9-4d68-84a2-e6d57d5c615b.png">

# Deliverable 4
  In the last deliverable we created scatter plots with Plotly Express and hvplot, in order to visualize the distinct groups that correspond to the three principal components you created in Deliverable 2. Next we created a table with all the currently tradable cryptocurrencies using the hvplot.table() function. Once we had our table created we used the MinMaxScaler().fit_transform method to scale our columns between zero and one. This then allowed us to create another DataFrame we could plot using the hvplot scatter plot. 

<img width="430" alt="Screen Shot 2023-04-03 at 4 08 25 PM" src="https://user-images.githubusercontent.com/117120227/229645763-6a88caba-3fe0-450a-a922-cd8691c54f92.png">

