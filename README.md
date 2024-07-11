# MySQL Advanced Techniques

## Table of Contents

- [Introduction](#introduction)
- [How to Create Tables with Constraints](#how-to-create-tables-with-constraints)
- [How to Optimize Queries by Adding Indexes](#how-to-optimize-queries-by-adding-indexes)
- [What is and How to Implement Stored Procedures and Functions in MySQL](#what-is-and-how-to-implement-stored-procedures-and-functions-in-mysql)
- [What is and How to Implement Views in MySQL](#what-is-and-how-to-implement-views-in-mysql)
- [What is and How to Implement Triggers in MySQL](#what-is-and-how-to-implement-triggers-in-mysql)
- [Requirements](#requirements)
- [More Info](#more-info)
- [How to Import a SQL Dump](#how-to-import-a-sql-dump)

## Introduction

This project provides an in-depth guide on advanced MySQL techniques including creating tables with constraints, optimizing queries with indexes, and implementing stored procedures, functions, views, and triggers.

## How to Create Tables with Constraints

Constraints are rules enforced on data columns in a table to maintain the accuracy and reliability of the data. Common types of constraints include PRIMARY KEY, FOREIGN KEY, UNIQUE, and CHECK.

## How to Optimize Queries by Adding Indexes

Indexes are used to retrieve data from the database more quickly by providing a faster path to the data. Adding indexes can significantly improve the performance of read operations.

## What is and How to Implement Stored Procedures and Functions in MySQL

Stored procedures and functions are reusable SQL code blocks stored in the database. They can encapsulate complex logic, improve performance by reducing client-server communication, and ensure consistent implementation of business rules.

## What is and How to Implement Views in MySQL

Views are virtual tables representing the result of a database query. They provide a way to simplify complex queries, enhance data security by restricting access to specific rows or columns, and present data in a particular format without altering the underlying tables.

## What is and How to Implement Triggers in MySQL

Triggers are automated actions that are executed in response to certain events on a table, such as INSERT, UPDATE, or DELETE. They are used to enforce business rules, maintain audit trails, and synchronize tables.

## Requirements

### General
- All your files will be executed on Ubuntu 18.04 LTS using MySQL 5.7 (version 5.7.30)
- All your files should end with a new line
- All your SQL queries should have a comment just before the query
- All your files should start with a comment describing the task
- All SQL keywords should be in uppercase (e.g., SELECT, WHERE)
- A README.md file at the root of the project folder is mandatory
- The length of your files will be tested using the `wc` command

## More Info

### Comments for your SQL file:
Include comments in your SQL files to describe the purpose of the queries and the logic behind them. This will help others understand your code and maintain it in the future.

### Use "container-on-demand" to run MySQL
- Request a container with Ubuntu 18.04 and Python 3.7
- Connect via SSH or WebTerminal
- Start MySQL in the container before using it:
  - Use `service mysql start` to start the MySQL server

### In the Container, Credentials are `root/root`
- Use these credentials to log into MySQL and execute your SQL scripts

## How to Import a SQL Dump

1. Create a database to import the SQL dump into.
2. Download and import the SQL dump using `curl` and pipe it to the `mysql` command.
3. Verify the import by querying the relevant tables.