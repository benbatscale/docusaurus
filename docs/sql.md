---
id    : sql
title : MySQL
---

## General Knowledge

* A statement in SQL is like a sentence in English.
* A query in SQL is like asking a question in English.
* Relational DB comes from their usage in comparing the relationship between 2 values.


## Cheatsheet
* **SELECT * FROM <table_>;**
* **SELECT <col_> FROM <table_>;**
* **SELECT <col_> AS <alias> FROM <table_>;**
* **SELECT <col_> FROM <table_> WHERE <col_> = <val_>;**
* **SELECT <col_> FROM <table_> WHERE <col_> = <val_> AND[OR] <col_> < <val_>;**

## Basic Queries

*What is all the info we have about each patron in the patrons table?*
* **SELECT * FROM patrons;**

*Find all emails or first_name from the patrons table*
* **SELECT email, first_name FROM patrons;**

*Alias phone column with the word "number"*
* **SELECT phone AS "number" FROM patrons;**

*What are all first name and last names of the patrons that are born in 1987?*
* **SELECT first_name, last_name FROM patrons WHERE dob = 1987;**
* **SELECT phone FROM patrons WHERE first_name = "Ashley";**

*Find all patrons with first name John and last name Appleseed*
* **SELECT * FROM patrons WHERE first_name = "John" AND last_name = "Appleseed"**

