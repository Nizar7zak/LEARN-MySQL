# LEARN-MySQL
here is everything you want to learn about the world's most popular open source database.


## Introduction
This Repo is Ideal for any one who wants to learn SQL from scratch, but also anyone with some basic knowledge who wants to fill in the missing gaps.

By the end of this repo, you'll be able to **retrive**, **insert**, **update** and **delete** data in databases.

We'll talk about tables, **relationships**, different type of joints, sub-queries, regular expressions and much more. These are the essential concepts every software developer or data scientist must know. 
In this repo you will face many exercises that help you both learn and remember the **SQL** syntax.


## What is a Database? 
Let's start with a quick overview of databases, what they are? and how we use them?

**A database is a collection of data stored in a format that can easily be accessed.**

In order o manage our databases, we use a software application called `Database Management System` or **DBMS**. We connect to a DBMS and give it instructions for querying or modifiying data. The DBMS will execute our instructions and send results back. 

![](https://i.imgur.com/mb41Ku8.png)


Now we have several databases management systems out there, and these are classified into two categories, **Relational** *SQL* and **Non-Relational** *NoSQL* 

In relational databases we store data in tables taht are linked to each other using relationships. That's why we call these databases relational databases.
Each table stores data about a specific type of object like Customer, Product, Order and so on.

![](https://i.imgur.com/AufGgaP.png)


## SQL - STRUCTURED QUERY LANGUAGE
SQL is the langauage that we use to work with these relational database management systems. We use SQL to query or modify our data. It looks like this:-

```
SELECT *
FROM products
WHERE category = 'food'
ORDER BY price
```

There are many different relational database management systems, some of the most popular ones are :-
* **MySQL**
* **SQL Server**
* **Oracle**
* **POSTGRESQL**

Each DBMS has a different flavor of SQL, but all these implementations are very similar and are based on the standard SQL specification. So most of the SQL code that you will learn here, will work with any DBMS.

## What about NoSQL?

In non-relational databases, we don't have tables or relationships, these databases are very different from RELATIONAL databases, but that's a topic for an entirely different course.

What you need to know is non relational database management systems **don't understand SQL**. They have thier own query language. So, we use **SQL** to work with **RDBMS**  

