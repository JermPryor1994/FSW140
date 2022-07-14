# FSW 140 Weeks 1-3 Lecture

## Agenda

1. Introductions
2. Problem Solving Process
3. How to Ask a Good Question
4. Intro to Relational Databases
5. Intro to SQL
6. Where and How to Learn
7. Q & A

## Overview

This course leans heavily on the associated e-book and I highly suggest you keep up with or get ahead with the assigned readings. Most of the exercises and assignments are taken from the book so please use that as your main resource.

We will be meeting for lecture on Friday July 1st for our weeks 1 & 3 lecture, Friday July 15th, and Saturday July 30th for weeks 5 and 7 respectfully. My office hours are even weeks (weeks 2, 4, 6, 8) on Wednesdays at 5 pm (PT).

### Learning Goals

In this lesson we:

- Will explore, at a high level, both relationala nd non-relational databases
- Be introduced to Structured Query Language (SQL)
- Re-solidify our understand of where these queries take place in our HTTP REQ <-> RES Cycle

## 1. Introductions

## 2. Problem Solving Process

Starting and maintaining a good problem solving process is a **vital** skill as a programmer. This is especially important for students and soon to be junior level devs.

The key here is to find something that works for you and stick to it no matter what. As the idium goes, "3 hours of planning can save you 3 days of headaches."

### Ex: The 20 min rule

Conceptually, we never want to be stuck on a given problem for more than 20 minutes. Let's take a look at that practically.

1) Given any problem or task the first step will always be to map out your direction, idea, data strucure & flow, components, local & global state, folder structure, required modules, ...etc. This can be quick but is vital to our process. Should be done with psedo code and some form or drawings or wireframing.

2) Code out the scaffold of your project and start working on your tasks, constantly testing or reffering to the unit tests provided to you. Important to do this as you develop (Test Driven Development) not once you complete hours of coding.

3) When stuck try different solutions for no more than 20 mins in your IDE. DO NOT use destructive code — meaning comment out old code not deleting it in lie of copy pasting new code from the internet. Creating this breadcrumb of ideas 99% of the time will lead you to your answer before moving forward.

4) Take a break! This can mean any number of things I usually suggest to go work on other code. Something that is "easy" or "easily" completed in your project. Often times writing sucessfull code can get your brain flowing again. Or go for a walk, do some pushups, find your peace, take the dog out — whatever works for you.

5) Try again for 20 minutes. You should not have went through stack overflow or anythign yet if you are goign to use outside materials it should be from your notes or the **documentation** for whatever you are using. I know often your answer can be found easily on SO but at your level I think it will help you immensely to try and figure it out without that help. Leading to a stronger knwledge base will make your interview process easier and ultimately add more value to the first company you go to work for.

6) Leave comments **everywhere**. If you are not, start immediately and do not stop. This is important for your own sanity but also good practice for when you join a team. Think of facebooks codebase and 100,000 some developers globally. Imagine looking at some code and trying to figure out a bug or what the problem is with no test files or comments. Write comments everywere. Full stop. This will also differenite your code from other juniors as you move into the interview process.

7) If you can not figure it out yet now head online in this order — documentation, blogs/vids/articles, stack overflow. When using google for these look for **recent** posts.

8) If you are still stuck you need to ask somebody for help. Utilize your networks. Start thinking about the fact you will not have this BU network soon and begin thinking about how to create your own moving forward. Twitter, dischords, slack channels, meetups.

## 3. How To Ask a "Good" Question

Asking a good question is not only for yourself but helps the person helping you quickly and efficently figure out what in the hell is going on in your jumbled mess of a project and how to help you through it. At first this will be your support system at BU, next most likely stack overflow, and lastly your mentor or senior level devs. The very first thing your senior dev will ask you will be did you google it.

### Contents of a "good" question

1) Code snippets of every file involved. If full stack MERN this could be 5-10 ... all labeled on the top with a comment of the name of the file. Including the commented out code of your "tries."

2) A description of the problem you are trying to solve, or what you are tryign to accomplish. Think — how do I do x ..... tell us what x is.

3) What you specifically have done to try and solve this problem.

4) What error you are getting and any associated screenshot of that error.

## 4. Intro to Databases

A database management system is a software package for creating and managing databases. Many different types of database systems exist based on how they manage the database structure.

    Relational vs. Non-Relational

A **relational database** contains multiple tables of data with rows and columns that relate to each other through special key fields. These databases are more flexible than flat file structures (non-relational), and provide functionality for reading, creating, updating, and deleting data. Relational databases use Structured Query Language (SQL) - a standard user application that provides an easy programming interface for database interaction. Common examples of this are mySQL, Oracle, Microsoft SQL Server, and PostgreSQL which you will be learnign about in a later course.

A popular alternative to relational databases, **non-relational databases** (NoSQL) take a variety of forms and allow you to store and manipulate large amounts of unstructured and semi-structured data. Examples include key-value stores, document stores, and graph databases.

An interesting aspect of a non-relational database such as NoSQL is scalability. NoSQL uses the **BASE** system (basically available, soft-state, eventually consistent). Non-relational databases forgo the table form of rows and columns relational databases use in favor of specialized frameworks to store data, which can be accessed by special query APIs. Persistence is an important element in these databases. To enable fast throughput of vast amounts of data the best option for performance is "in memory," rather than reading and writing from disks.

Relational databases use the ACID system, which ensures consistency of data in all situations of data management but obviously takes longer to process because of all those relations and its branching nature. However, the BASE system loosened up the requirements on consistency to achieve better availability and partitioning for better scalability.

## 5. Intro to SQL

SQL is a standard language for storing, manipulating and retrieving data in databases. Although SQL is an ANSI/ISO standard, there are different versions of the SQL language.

However, to be compliant with the ANSI standard, they all support at least the major commands (such as `SELECT`, `UPDATE`, `DELETE`, `INSERT`, `WHERE`) in a similar manner.

> Most of the SQL database programs also have their own proprietary extensions in addition to the SQL standard!

### RDBMS

RDBMS stands for Relational Database Management System.

RDBMS is the basis for SQL, and for all modern database systems such as MS SQL Server, IBM DB2, Oracle, MySQL, and Microsoft Access.

The data in RDBMS is stored in database objects called tables. A table is a collection of related data entries and it consists of columns and rows.

Every table is broken up into smaller entities called _fields_. A **field** is a column in a table that is designed to maintain specific information about every record in the table.

A _record_, also called a **row**, is each individual entry that exists in a table. A **record** is a horizontal entity in a table.

A **column** is a vertical entity in a table that contains all information associated with a specific field in a table.

### Statements

Most of the actions you need to perform on a database are done with SQL statements.

Some of The Most Important SQL Commands:

- `SELECT` - extracts data from a database
- `UPDATE` - updates data in a database
- `DELETE` - deletes data from a database
- `INSERT INTO` - inserts new data into a database
- `CREATE DATABASE` - creates a new database
- `ALTER DATABASE` - modifies a database
- `CREATE TABLE` - creates a new table
- `ALTER TABLE` - modifies a table
- `DROP TABLE` - deletes a table
- `CREATE INDEX` - creates an index (search key)
- `DROP INDEX` - deletes an index

## 6. Where and How to Learn

- [Kightlab](https://mystery.knightlab.com/)
- [Select Star SQL](https://selectstarsql.com/)
- [Microsoft SQL Workshops](https://microsoft.github.io/sqlworkshops/)
- [SQL Zoo](https://sqlzoo.net/)
- [SQl Tutorials](https://www.w3schools.com/sql/)

## Summary

### References

## 7. Questions
