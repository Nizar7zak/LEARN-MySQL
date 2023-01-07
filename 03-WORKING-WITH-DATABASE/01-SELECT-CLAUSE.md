# The SELECT Clause
**Now we're going to look at the SELECT clause in detail:-**


### What can we do with SELECT clause?
``` 
SELECT *
FROM customers;
```
* As you know, if you use an asterisk *, this will return all the columns. 
* Alternatively we can specify the columns that we want and this is helpful in situations where you have a **big table** with so many columns and perhaps millions of records.
* If you want to bring back all that data, that's going to put a lot of pressure on the database server.

Now let's say we want to get the first name and the last name.

```
SELECT first_name, last_name
from customers;
```
![](https://i.imgur.com/nmvZtAj.png)

As you can see, we only get these two columns. And thay are in the same order we specified.


```
SELECT last_name, first_name
from customers;
```

* So if you change the order and put the last name first and execute the query again, you should see the last name column comes first.

![](https://i.imgur.com/Z9C4mVw.png)

Now, let's add a new column at the end, let's get the points for each customer.

```
SELECT last_name, first_name, points
from customers;
```
![](https://i.imgur.com/gE4KYov.png)

As you can see, these are the points for each customer which are calculated based on thier shopping.

* Imagine we want to get these points and put them in mathematical formula to calculate the discount that we can give to each customer.this lead us to **Arithmetic expression!**

```
SELECT last_name, first_name, (points + 10) * 100
from customers;
```
As you can see, that's ```points + 10```. This is an **Arithmetic expression**. Now execute the query, you can notice every point will end up plus ten.
![](https://i.imgur.com/b6upRnU.png)

* **Note:-** you can rename ```(points + 10) * 100``` by using **AS** alias, look at the query below:-

```
SELECT last_name, first_name, points + 10 AS discount_factor
from customers;
```
![](https://i.imgur.com/HlAZybq.png)


---
## Unique list:-
* Try to change the first record in customers table - state column to **VA**. Now the first and second record have a **VA** state.


### How we can get a unique list of state?
This can be done by use a **DISTINCT** keyword like this:-

``` 
SELECT DISTINCT state
FROM customers 
```


---

* EXERCISE

```
Retrun all the products
name 
unit price
new price = unit price * 1.1
```