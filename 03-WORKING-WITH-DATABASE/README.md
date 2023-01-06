# The SELECT Statment

---

### What the meaning of QUERY?
***Is the answer or retrieved information comes from a database.***


---

### What the meaning of CLAUSE?
***Is a built-in function that is used to retrieve the data from the records present in the database.***


---


* Now we'll learn how to retrive data from a single table.
* The first step to write a query to get data from a database, is to select a database. Then the query that we'll write will be executed against that databse. 
> Here we're going to use **sql_store** database

* Write the following line of code, then execute it:- 
```
USE sql_store 
```
> USE is a keyword in the SQL language.

![](https://i.imgur.com/5QvtXEY.png)

Look! **sql_store** database is now displayed in bold-selected.

* **SQL** is not a case sensitive language, which means we can use upper case or lower case characters, it doesn't really matter, but as a best practice we should capitazlie the SQL keywords, and use lower case characters for everything else.


---

## Our First Query:-
Let's write our first query to retrive all the customers in this database.

* After the **USE** statment we're going to use the SELECT statment.

#### The basic Sructure of SELECT statment:-
```
SELECT column_name1, column_name2 
FROM table_name
```
> Instead of retrieve a specific columns, we can retrive all columns using an asterisk *

* Let's try to retrieve **all columns** from **customers table.**

```
USE sql_store ;
SELECT *
FROM customers;
```
> Whenever you have mutliple SQL statments like the piece of code above, you need to terminate each statment using a semicolon **;** as you see we wrote **;** after every SQL statment.

* Now let's execute our code and see the output, we can use the shortcut **(Ctrl+Enter)** to execute the current QUERY.

![](https://i.imgur.com/impdExk.png)

* This SELECT statment has two **clauses**:-
1. SELECT **clause**.
2. FROM **clause**.
* There are other clauses we can use to filter and sort data.

> we can use WHERE clause to filter the result and get the cusomter with ID=1


```
USE sql_store ;
SELECT *
FROM customers
WHERE customer_id = 1;
```

When we execute this query we'll only get the customer with **ID=1**

> we can also sort the data, use the **ORDER BY** clause and specify the column that we're going to sort the results depends on.

```
USE sql_store ;
SELECT *
FROM customers
ORDER BY first_name;
```

* We will back again to learn more about these clauses in details.
### Notes:- 
> * All the next Clauses **(FROM, ORDER BY, WHERE) are optinal, but in the real world we quite often use all of them.
> * The order of these clauses matter! so we always select first, then we have FROM, then WHERE and finally ORDER BY.
> * Otherwise we get a syntax error, which basically means the synatx or the grammar or the strucuture of our statment is incorrect. and can not be executed. 
> 
### Comment Out:-
To comment out any line of code we can use **--** before any line, these **--** will prevent the line from execution.

```
USE sql_store ;
SELECT *
FROM customers
--ORDER BY first_name;
```
