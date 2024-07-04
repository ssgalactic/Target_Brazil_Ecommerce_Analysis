# Target_Brazil_Ecommerce_Analysis
Analyzing Target's e-commerce operations in Brazil from 2016-2018 using SQL on Google BigQuery.
Target_Brazil_Sales_Analysis
Target is one of the world’s most recognized brands and one of America’s leading retailers. This business case has information on 100k orders from 2016 to 2018 made at Target in Brazil. Its features allow viewing an order from multiple dimensions.

Data is available in 8 CSV files:

customers.csv
geolocation.csv
order_items.csv
payments.csv
reviews.csv
orders.csv
products.csv
sellers.csv

Each feature or columns of different CSV files are described below: The customers.csv contains the following features: customer_id: Id of the consumer who made the purchase. customer_unique_id: Unique ID of the consumer. customer_zip_code_prefix: Zip Code of the location of the - consumer. customer_city: Name of the City from where an order is made. customer_state :State Code from where order is made(Ex- sao paulo-SP). The sellers.csv contains the following features: seller_id: Unique ID of the seller registered seller_zip_code_prefix: Zip Code of the location of the seller. seller_city: Name of the City of the seller. seller_state : State Code (Ex- sao paulo-SP) The order_items.csv contain following features: order_id: A unique id of order made by the consumers. order_item_id: A unique ID given to each item ordered in the order. product_id: A unique ID given to each product available on the site. seller_id: Unique ID of the seller registered in Target. shipping_limit_date: The date before which shipping of the ordered product must be completed. Price: Actual price of the products ordered. freight_value: Price rate at which a product is delivered from one point to another. The geolocations.csv contains the following features: geolocation_zip_code_prefix: first 5 digits of zip code geolocation_lat: latitude geolocation_lng: longitude geolocation_city: city name geolocation_state: state The payments.csv contains following features: order_id: A unique id of an order made by the consumers. payment_sequential: sequences of the payments made in case of EMI. payment_type: mode of payment used. (Ex-Credit Card) payment_installments: number of instalments in case of EMI purchase. payment_value: Total amount paid for the purchase order. The orders.csv contains the following features: order_id: A unique ID of an order made by the consumers. customer_id: ID of the consumer who made the purchase. order_status: status of the order made i.e delivered, shipped etc. order_purchase_timestamp: Timestamp of the purchase. order_delivered_carrier_date: delivery date at which the carrier made the delivery. order_delivered_customer_date: the date on which the customer got the product. order_estimated_delivery_date: estimated delivery date of the products. The reviews.csv contains the following features: review_id: Id of the review given on the product ordered by the order id. order_id: A unique ID of an order made by the consumers. review_score: review score given by the customer for each order on a scale of 1–5. review_comment_title: Title of the review review_comment_message: Review comments posted by the consumer for each order. review_creation_date Timestamp of the review when it is created. review_answer_timestamp: Timestamp of the review answered. The products.csv contains ins following features: product_id: A unique identifier for the proposed project. product_category_name: Name of the product category product_name_lenght: length of the string which specifies the name given to the products ordered. product_description_lenght: description length written for each product ordered on the site. product_photos_qty: Number of photos of each product ordered available on the shopping portal. product_weight_g: Weight of the products ordered in grams. product_length_cm: Length of the products ordered in centimetres. product_height_cm: Height of the products ordered in centimetres. product_width_cm: width of the product ordered in centimetres.

Insights and Recommendations :

In the analysis of Brazil's e-commerce target, it's observed that Tuesdays, Mondays, and Wednesdays have a relatively higher number of orders. There is an increasing trend in orders, which sustained throughout 2018. There was a slight fall in October 2017 followed by a significant hike in November 2017, and again a fall in December 2017 and January 2018.

A significant increase in orders and revenue, 815% and 707% respectively, was seen from January 2017 to January 2018. However, the growth rate for July and August in 2017 and 2018 was relatively very low. The highest growing sale months compared to the previous month were February 2017, March 2017, and November 2017.

In the products data, a total of 32951 different products are available at Target across 73 different product categories. Health and beauty, watches, bed table bath, sport leisure, computer accessories, furniture decoration, housewares, and automotive are some of the top-selling product categories. Health and beauty products are top-selling with the highest number of orders.

PCs and musical instruments categories have a relatively low number of products but contribute significantly to revenue. Categories with the highest average product prices are PCs, house pastels oven and cafe, agro industry and commerce, musical instruments, and kitchen portable and food coach. 61% of orders fall within the price range of 10-100, and 33% are in the 101-500 price range.

PCs/electronics, furniture products, kitchen service area dinner and garden equipment, industry commerce and business, agro-industrial commercial products, bags accessories, musical instruments, and construction tools illumination are some product categories with high average freight values.

In terms of delivery time, the average time for approving the order by the seller is 0.26 days, with a median time of 0, which means within a day. The average time taken by a carrier to start the delivery is 2.5 days, and the average time taken to complete delivery is 12 days, with a median of 10 days. The estimated average delivery time is 23 days. There is a positive correlation between freight value and delivery time.

States such as São Paulo, Paraná, Minas Gerais, Distrito Federal, Santa Catarina, and Rio de Janeiro have faster delivery times. On the other hand, Alagoas, Amazonas, Amapá, Pará, and Roraima have relatively slower delivery times.

In terms of region and state-wise analysis, São Paulo, Rio de Janeiro, Minas Gerais, Rio Grande do Sul, and Paraná are the top 5 states with the highest number of orders and revenue. More than 80% of orders and 90% of revenue are coming from the south, southeast, and northeast regions of Brazil.

Based on the distribution and statistical analysis, it's observed that the average delivery time is 12 days, which should be reduced to at least half due to high competition in the e-commerce market. To achieve this, the average time for the carrier to start delivery (2.5 days) and the order approval time (0.26 days) should be optimized to as low as possible.

It was also recommended to increase the network in the north of Brazil to increase the customer base. Introducing necessary products for survival, camping, and adventure can help increase revenue and orders from the northern region. Additionally, offering discounts on slower moving products may help to boost sales during low months such as October and January.

Please remember the following points:

- The period for which the data is given is 25 months.
- Compared to 2017, revenue has increased in 2018 by 21%.
- The average number of orders is higher during November, Monday, and Wednesday, while September and October have comparatively lower average orders. May, July, and August have higher average orders compared to other months.

Increasing trend:

- There is an increasing trend in orders, which sustains during 2018. There is a slight fall in October 2017, followed by a significant spike in November, and again a fall at the end of December 2017 and January 2018.
- We can observe the trend of increasing orders with time and also for revenue.
- There was an 815% growth in orders and a 707% growth in revenue in January from 2017 to 2018.
- The growth rate for July and August from 2017 to 2018 is relatively very low.
- February 2017, March 2017, and November 2017 were the highest growing sale months compared to their previous months.

In the Products Data section:

- There are a total of 32951 different products available in Target with 73 different product categories. Health and beauty, watches, bed table bath, sport leisure, computer accessories, furniture decoration, housewares, and automotive are some of the top-selling product categories.
- Health and beauty products are the top-selling products with the highest number of orders.
- PCs and Musical Instruments categories have a relatively fewer number of products but contribute to high revenue.
- PCs, house pastals oven and cafe, agro industry and commerce, musical instruments, kitchen portable and food coach are the categories with the highest average product prices.
- 61% of orders are between the price range of 10-100, and 33% are from the 101-500 price range.
- PCs/electronics, furniture products, kitchen service area dinner and garden equipment, industry commerce and business, agro industrial commercial products, bags accessories, musical instruments, and construction tools illumination are some product categories with high average freighter value.

Delivery time:

- Average estimated delivery time and delivery time have a positive correlation with average freight value.
- After purchasing, the average time for approving the order by the seller is 0.26 days, and the median time is 0, which means within a day.
- The average time taken for a carrier to start the delivery is 2 and a half days.
- The average time taken to complete a delivery is 12 days, and the median delivery time is 10 days.
- The average estimated delivery time is 23 days.
- There is a positive correlation between freight value and delivery time.
- São Paulo, Paraná, Minas Gerais, Distrito Federal, Santa Catarina, and Rio de Janeiro are some of the states where delivery is relatively faster.
- Alagoas, Amazonas, Amapá, Pará, and Roraima are states that have very slow delivery times relatively.

Region and State-wise Analysis:

- São Paulo, Rio de Janeiro, Minas Gerais, Rio Grande do Sul, and Paraná are the top 5 states with the highest number of orders and also generating the highest revenue. More than 80% of orders and 90% of the revenue are coming from the south, southeast, and northeast Brazil.

Recommendations:

- From the distribution and statistical analysis, we can observe that the average time to complete delivery is 12 days. This should be reduced to at least half, as due to high competition in the e-commerce market, it is vital to do so.
- In order to reduce the delivery time, if we look at the average time for the carrier to start the delivery, it takes at least 2 and a half days. The order approval time is 0.26 days. These two should be optimized as low as possible to result in faster deliveries.
- Delivering faster in the northern states may create and increase new customers and revenue from the north.
- Increasing the network in North Brazil, especially in small towns, can help increase the customer base. Introducing necessary survival/camping/adventure products can help increase revenue and orders from the northern region.
- Introducing discounts on less popular products can help sell more during slower months such as October and January.

