Market Basket Analysis Using Instacart Online Grocery Dataset -Project

Tasks to be performed: 
Task 1: Explore the orders dataset and create a dataframe
 <img width="1414" height="505" alt="image" src="https://github.com/user-attachments/assets/22f136bc-3cd0-42ca-9b7a-76a95efd4e3a" />

Steps to perform:
1. Read the orders data as a dataframe in pySpark  Note: The column days_since_prior_order may contain some NULL values.  
2. Display the data up to 10 rows
 <img width="1414" height="916" alt="image" src="https://github.com/user-attachments/assets/f78f82f7-8a21-4c01-aea4-c366f8b032cb" />


Task 2: Replace all the null values 
Aim: To delete existing Null values 
Steps to perform: 
1. Replace all null values with a dummy 999 value in the dataframe that was created in task 
2. Show top 10 records
 <img width="1414" height="563" alt="image" src="https://github.com/user-attachments/assets/d24c5caf-0876-4534-8ac5-636166d18a11" />



Task 3: Identify the busiest day 
Aim: To examine the order information and find the busiest day of the week by reading the data as a pySpark dataframe 
Steps to perform: 
1. Read the orders.csv data stored in HDFS
2. Store the table for a particular spark session 
3. Compute the total number of orders as Total_Orders placed on each day of the week 
Hint: The column order_dow represents the day of the week 
Wherein: 
Day 0 is Sunday 
Day 6 is Saturday and so on 
4. Display the result that contains the total orders placed on each day of the week (Monday to Sunday)
<img width="1414" height="910" alt="image" src="https://github.com/user-attachments/assets/783268fc-04ff-46e6-9fc8-7e4a3d81a6ce" />


 

Task 4: Calculate the busiest hour 
Aim:  Give a breakdown of orders by the hour 
Steps to perform: 
1. Read the orders.csv data stored in HDFS 
2. Store the table for a particular spark session 
3. Select the number of order IDs as Total_Orders and the hour at which the 
order was placed using spark sql 
4. Display the result that contains total orders and the hour 
 <img width="1414" height="905" alt="image" src="https://github.com/user-attachments/assets/fb54854f-1432-465b-b11b-72aceda48118" />


Task 5: Identify the most popular item 
Aim:  To identify the top 10 popular items 
Steps to perform: 
1. Read the order_products__prior.csv and products.csv data 
2. Store the tables for a particular spark session 
3. Calculate the top 10 popular items based on the count of orders
4. Display the result that contains the product name as  Popular_product_name and the count of order id as Order_Count

 <img width="1350" height="597" alt="image" src="https://github.com/user-attachments/assets/a2b518a0-a3d1-4bb4-ba9a-b2c8409762d4" />

 <img width="1350" height="525" alt="image" src="https://github.com/user-attachments/assets/24016f7b-00a7-435e-af2a-4883d0eade59" />



Task 6: Explore the department dataset and create a dataframe 
Aim:  Read the department CSV as a pySpark dataframe 
Steps to perform: 
1. Read the data from the departements.csv file 
2. Display the data stored

Task 7:  Display the department id that has published maximum products

<img width="1350" height="835" alt="image" src="https://github.com/user-attachments/assets/2d113703-5813-4bf0-8c8c-f4e8c83b3f98" />

 




