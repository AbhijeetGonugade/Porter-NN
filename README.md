# Porter-NN
Process 
1. Import the data and understand the structure of the data: • usual exploratory 
analysis steps like checking the structure & characteristics of the dataset 
2. Data preprocessing • Cleaning of data • Feature engineering: Creating the target 
column time taken in each delivery from order timestamp (created_at) and 
delivery timestamp (actual_delivery_time) • Getting hour of day from the order 
time and also the day of the week • Understanding pandas datetime data type 
and what function it provides by default • Get delivery time in minutes 
3. Handling null values 
4. Encoding categorical columns 
5. Data visualization and cleaning • Visualize various columns for better 
understanding Countplots, scatterplots 
6. Check if the data contains outliers • Removing outliers by any method • Plotting 
the data again to see if anything has improved 
7. Split the data in train and test 
8. Scaling the data for neural networks. 
9. Creating a simple neural network • Trying different configurations • 
Understanding different activation functions, optimizers and other 
hyperparameters. 
10. Training the neural network for required amount of epochs 
11. Plotting the losses and checking the accuracy of the model 
12. Checking its various metrics like MSE, RMSE, MAE 
Google colab link:  
https://colab.research.google.com/drive/1HP6bQPYu7dXSdXWqr5f2C3v21c_V5vRu?usp=sharing

Dataset: https://d2beiqkhq929f0.cloudfront.net/public_assets/assets/000/015/039/original/dataset.csv.zip?1663710760

Data Dictionary

Each row in this file corresponds to one unique delivery. Each column corresponds to a feature as explained below.

market_id : integer id for the market where the restaurant lies
created_at : the timestamp at which the order was placed
actual_delivery_time : the timestamp when the order was delivered
store_primary_category : category for the restaurant
order_protocol : integer code value for order protocol(how the order was placed ie: through porter, call to restaurant, pre booked, third part etc)
total_items subtotal : final price of the order
num_distinct_items : the number of distinct items in the order
min_item_price : price of the cheapest item in the order
max_item_price : price of the costliest item in order
total_onshift_partners : number of delivery partners on duty at the time order was placed
total_busy_partners : number of delivery partners attending to other tasks
total_outstanding_orders : total number of orders to be fulfilled at the moment
