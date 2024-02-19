# BI_DA-Brazil-Ecommerce
Dataset Link: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce


## 1. Description
   
The dataset includes information about 100,000 orders made at Olist Store, the largest e-commerce platform in Brazil. After a customer purchases a product from Olist Store, the seller will receive a notification to fulfill that order. Once the customer receives the product or the estimated delivery date is due, the customer will receive an email satisfaction survey where they can take notes about their purchase experience and write down some feedback.

Data will include information related to customers, products, shipping, payments, revenue... of orders. Our ultimate goal is to build a complete Business Intelligence model for relevant data and find useful insights from analyzing cleaned, selected and modeled data.

## 2. Tasks

- Perform ETL to clean and extract data from database into Data Warehouse.

- Conduct data modeling and visualization to discover existing problems in the enterprise's business processes.

## 3. Detailed Visualization and Data Analysis
### 3.1. Sales overview

Master dashboard
- The total sales, total orders are 13,59 million R$ and 99 thousand orders respectively,  and have increased significantly since 2017, with the highest sales in 11/2017.
- The average order value is 137,75 R$
- The cancellation rate is only 0,47%, which is a positive sign.
- The best selling products of all time are health and beauty products.

Highest Sales Date
Drilling into 11/2017, it was obvious why this month yielded the greatest sales. Black Friday was the 24th of the month, orders and sales exploded during this day. 

Customer Segments’ Distribution
Customers are divided into 4 segments by using the RFM metrics. However, the datasets that were provided only consist of customers that either have made a purchase once or have never purchased anything, the F (Frequency) metric is therefore left out. Customers are then segmented by using only the R (Recency) and M (Monetary) metrics. Those who have made a purchase recently that is also one of high-value are the “VIP Shoppers”, those who made a purchase of high-value but haven’t purchased again recently are the “Past High Rollers”. Those who ordered moderate-value products recently are the “Recent Buyers” and those who have only made a purchase of low-value products a long time ago are the “Inactive Customers”.
Low to moderate-value customers are about 60% of the customer base but only account for 25% of sales .“VIP Shoppers” and “Past High Rollers” on the other hand, take about 40% of the customer base but account for 75% of sales, these are the customers that the company needs to focus more with their marketing efforts.

### 3.2. Customer Segments’ preferences
#### 3.2.1. Inactive Customers and Recent Buyers

Inactive Customers’ preference

Recent Buyers’ preference
These 2 types of customers are not so different on their taste and behavior, they share some common characteristics:
- They tend to make purchases during weekday afternoons.
- The value of their orders are not substantial so they want to pay up quickly, preferably within 3 installments. 
- They have a liking for items like bed-bath-table (which are home appliances), health and beauty cosmetics, sports and leisure-related products.

#### 3.2.2. VIP Shoppers and Past High Rollers

VIP Shoppers preference

Past High Rollers’ preference
These 2 also have similar patterns in their favorite ordering time as the 2 types above as they prefer to make a purchase during weekday afternoons. VIP Shoppers especially are most active on Monday afternoons.
Aside from that, these 2 types are alike in these traits:
- They love buying watches and gifts, apart from the common favorites.
- They tend to pay within 5 installments, probably because of the high value items.
The 4 segments are not separable by payment methods, as they all primarily pay with credit cards.

### 3.3. Product Reviews

Product Reviews
Some statistics about product reviews:
- 40,77% of order reviews had a comment included.
- 77% of reviews were positive, which had a rating of either 4 or 5.
- cds-dvds-musicals had the highest average rating of 4,64 while security and services had the lowest average rating of 2,50

### 3.4. Delivery time

Delivery Time & Reviews
Delivery time statistics:
- The average confirmation time is 0,53 days, the average pickup time is 2,75 days, the average delivery time is 9,14 days. From start to end (purchasing to receiving), the process took 12,41 days on average.
- 8,11% of orders were late
One key takeaway is that the delivery time does affect the customers’ satisfaction: the slower the delivery time, the lower the review score. That’s why we will need to look at specific sellers, cities or states that are having delivery problems.

States, Cities and Sellers
States and cities that have a percentage of late orders over the average number would be marked with a red icon. Considering the top 3 states that generate the highest sales, we have RJ (Rio de Janeiro) quite out of standard so we would look at this state in specific to uncover the underlying issues.

Rio de Janeiro’s delivery situation
Looking at the figure, almost all the cities in this state are having a problem with delivering orders on time. The sellers are obviously not at fault here since the confirmation time and pickup time was relatively short while the time to pickup and deliver an order took ages to complete.

## 4. Recommendations
### 4.1. Consider peak sales time
- Special days like Black Fridays or other holidays are a must for marketing strategies in order to increase product sales.
- Organize campaigns during weekday afternoons since this is the time that customers are active the most.
- 
### 4.2. Targeted marketing based on customer segments
- For the “Inactive Customers” and “Recent Buyers” groups
+ Consider boosting marketing efforts on bed-bath-table, beauty cosmetics, sports and leisure-related products.
+ Release vouchers that encourage installments in 3 months since this is their preferred duration to pay off an order
- For the “VIP Shoppers” and “Past High Rollers”:
	+ Focus more on these 2 groups than the previous 2 since they generate more sales.
+ Consider boosting marketing efforts on watches and gifts, basically luxury items and beauty products.
+ Release vouchers that encourage installments in 5 months since this is their preferred duration to pay off an order
- For “VIP Shoppers” specifically, consider releasing any kinds of vouchers or exclusive deals that would be in effect on Mondays as this is their favorite day to shop.

### 4.3. Products’ Quality Control
Look into sellers who sell diapers and hygiene, security and services products to see why they are getting negative reviews. Try to resolve the problem by contacting the seller and enforce measures to check their products’ quality. There might be fraudulent activities going on with the sellers who sell those kinds of products.

### 4.4. Address delivery issues
- A great number of states and cities were below standard in delivery time, especially Rio de Janeiro. This problem could lie in resource allocation. It seems that the company did not have enough warehouses or shipping units available in Rio de Janeiro, which led to a huge number of late deliveries.
- Perhaps they should consider searching for other transportation providers or have a direct meeting with the current partners to see what problems they encountered.
- If this issue could not be solved in a timely manner, consider providing customers that did not receive their package on time with compensation like vouchers or promotional offers.
