# Food-delivery-time
Food delivery time
To predict the Online Food Delivery time using machine learning algorithm depending various factors

Food Delivery services like Zomato and Swiggy need to show the accurate time it will take to deliver your order to keep transparency with their customers. These companies use Machine Learning algorithms to predict the food delivery time based on how much time the delivery partners took for the same distance in the past.

Dataset is uploaded from Kaggle.

To predict the food delivery time in real-time, we need to calculate the distance between the food preparation point and the point of food consumption. After finding the distance between the restaurant and the delivery locations, we need to find relationships between the time taken by delivery partners to deliver the food in the past for the same distance.So, for this task, we need a dataset containing data about the time taken by delivery partners to deliver food from the restaurant to the delivery location.

Initially Imported the necessary Libraries like, Numpy, Pandas, Plotly etc. The dataset doesn’t have any feature that shows the difference between the restaurant and the delivery location. All we have are the latitude and longitude points of the restaurant and the delivery location. We can use the haversine formula to calculate the distance between two locations based on their latitudes and longitudes. 

**Data Exploration is done by:**
1. Relationship Between Distance and time taken:There is a consistent relationship between the time taken and the distance travelled to deliver the food. It means that most delivery partners deliver food within 25-30 minutes, regardless of distance.
2. Relationship between distance and time taken on Person age of delivery person:There is a linear relationship between the time taken to deliver the food and the age of the delivery partner. It means young delivery partners take less time to deliver the food compared to the elder partners.
3. Relationship between Distance and time taken based on rating:There is an inverse linear relationship between the time taken to deliver the food and the ratings of the delivery partner. It means delivery partners with higher ratings take less time to deliver the food compared to partners with low ratings. 
4. Relation based on time taken in accordance with Vehicle used to delivery: So there is not much difference between the time taken by delivery partners depending on the vehicle they are driving and the type of food they are delivering.

So the features that contribute most to the food delivery time based on our analysis are:

>age of the delivery partner
>ratings of the delivery partner
>distance between the restaurant and the delivery location

Further train a Machine Learning model using an LSTM neural network model for the task of food delivery time prediction. Thus by Entering the above mentioned following details one can estimate the time required to delivery the online food delived.
