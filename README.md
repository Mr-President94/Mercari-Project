# Mercari Dataset Price Suggestion and Modelling

### Note that this project is a result of commendable group efforts from -

**1. Raghavendra Srinivasan**

**2. Raj Waje**

**3. Rohit Amalnerkar**

**Mercari** is an online shopping marketplace which is powered by one of the biggest community of Japan where users can sell pretty much anything.The community wants to offer price suggestions to the sellers but is a tough task as the sellers are enabled to put just about anything, or any bundle of things, on Mercari’s marketplace.


### Problem Statement:
- It can be hard to know how much something’s really worth. Small details can mean big differences in pricing. For example, one of these sweaters cost 335 dollars and the other cost 9.99 dollars. Can you guess which one’s which?

**Sweater A:** Vince, Long sleeve, Turtle neck pullover sweater, Black, Size L, Great condition

**Sweater B:** St. John's Bay Long sleeve, Turtle neck Pullover sweater, Size L, Great condition

- Hence, it's harder to guess or decide what price which product should have

- Product pricing gets even harder at scale, considering just how many products are sold online. Clothing has strong seasonal pricing trends and is heavily influenced by brand names, while electronics have fluctuating prices based on product specs.



### Challenges to Solve:

- Given details about a product like product category name, brand name, and item condition, our challenge is to build an algorithm that automatically suggests the right product prices

- But if solved rightly, it can eliminate human interference in giving price suggestions of a product and speed up efficiency of the shopping app. That’s when Machine Learning comes to play.

- The task of this Project is to build an algorithm that suggests the right product prices for shopping app from product name, user inputted text descriptions of the product, category name, brand name, item condition, and shipping information.

- The goal is about creating a model that would help sellers to price their products.Pricing should be intermediate between sellers and buyers.


### Our Objectives:

1. • Data Cleaning
    • Pre-processing
	• Feature Engineering 
2. Exploratory Data Analysis:
    - Gathering as many insights as possible through Exploratory Data Analysis. 
    - Trying to see through Descriptive Statistics that what our data is trying to tell us and understand the significance of each and every variable. 
3. Text Processing:
    - Natural Language Processing (NLP)
    - Tokenizing and tf-idf algorithm
    - K-means Clustering
5. The given problem is exactly about predicting the price, which is a real-valued value, thus it falls into the Regression Category
5. Trying to provide some interpretability and evolving our ways to handle the upcoming problems as we proceed through our project


### Models used in the Project:
1. Orinary Least Squares Regression
2. Linear Regression 
3. Ridge Regression  
4. Stochastic Gradient Descent Regressor     
5. Random Forest Regressor


## Data Description:

- `train_id` - the id of the product 

- `name` - the name of the product

- `item_condition_id` - the condition of the product provided by the seller
    
 According to information available on Mercari Website
    - 1 stands for new
    - 2 stands for fairly new
    - 3 stands for Good
    - 4 stands for Bad
    - 5 stands for Very Poor
    

- `category_name` - category of the product

- `brand_name` - brand name of the product

- `price` - the price that the product was sold for. (This is the target variable that we will predict) The unit is USD

- `shipping` - 1 if shipping fee is paid by seller and 0 by buyer

- `item_description` - the full description of the item


**Independent variables:** `train_id, name, item_condition_id, category_name, brand_name, shipping, item_description`

**Target Variable:** `price`

We will build various supervised machine learning regression models and see which succeeds in solving the given mapping between the input variables and the price feature in the best way.
