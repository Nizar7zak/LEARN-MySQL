# Creating the Databases
### Now we will know how to create the databases!

* open **MySQL workbench**, then connect to the database SERVER.

* Try to explore the interface of **MySQl workbench**
![](https://i.imgur.com/PnKqaa2.png)

* Don't worry! the first time you open it, it might appear alittle bit intimidating, but actually it's not that difficult.

* Try to explore the **tool bar**.
* On the left side, we've got the navigator panel with two tabs.
1. **Administration**:- we use the administration tab to do administrative work, such as starting or stopping our server, Importing data and so on.


2. **Schemas**:- The Schemas tabs shows the databases that we have in the current database server.



## Create the first Database
* To create the database for our project download [this file](https://drive.google.com/file/d/1qOxG3w9nzws8BJpOgr1ebY3ld-Iyp9Au/view?usp=share_link)
* Back to **MySQL** workbench and open the main SQL file
* Now excute the code and try to explore it.

### As you see, in every database we have objects:- 
1. **Tables**:- This is where we store our data.
2. **Views**:- We can think of views as a powerful tool for reports, because we can combine data from multiple tables and put them in a view.
3. **Stored Procedures**
4. **Functions**:- these are little programs that we stored inside of our databse for qureying data.

> For example you can have a store procedure for getting all the customers in a given city. So we call that procedure and we say:- **Give me all customers in GAZA, and this will return all the customers in GAZA.**


---

## let's Explore our tables!
### 1. Customers TABLE:-
![](https://i.imgur.com/REOeKy4.png)
* We have these columns like **customer_id which we use to uniquely identify customers** we also have first_name, last_name, and so on.
* Every row is called a **RECORD**. So every row represents one cutomer and these are the pieces of information we know for each customer


---

### 2. Orders TABLE:-
![](https://i.imgur.com/pSAhktd.png)

* We have these columns like order_id, customer_id, order_date, status, and so on.


> What is this customer_id in this table?

* We use this column **(customer_id)** to identify who has placed each order. What is interesting here is you have **referred** to this customers using thier cusomer_id, **which uniquely identifies that.**

> Why is that?
* It is possible one customer might have placed multiple orders in our App. Every time The customer places his order, we need to look up his address and phone to ship his order. 
* Now it is possible that some of this information might change in the future. The customer might move to new place or change his phone number, he might even change his name, if you repeat all that information next to each order, then we will have to come back and make changes in multiple places.
* In contrast, with this desgin we only store the ID of the customer here, so anytime we want to change any information about the customer, instead of changing that here, we go back to our customers table, and here this is the only place that we need to modify, so This is how **RELATIONAL DATABASE WORK!**


---

## Conclusion
* That basically means in these kind of databases we have multiple tables that are related to each other using a relationship. So internally there is a relationship between the customers table and the orders table. 
* The customer_id column in the customers table is linked with the customer_id column in the orders table.

### This is a brief intoduction to RELATIONAL databases.


* Exercise:- explore the **sql_invoicing** database.
