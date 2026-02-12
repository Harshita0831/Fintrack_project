# FINTRACK PRO – CLI Finance Manager

A command-line based personal finance management system built using Python, SQLite, and SQLAlchemy ORM.

This project allows users to track expenses, categorize spending, manage monthly budgets, and generate financial analytics using both ORM and raw SQL queries.

 #Project Overview

FinTrack Pro is designed to help users:

Track daily expenses

Organize expenses by category

Set monthly budgets

Monitor overspending

Generate category-wise analytics

The system demonstrates practical implementation of database design, ORM concepts, foreign keys, and SQL aggregation queries.

# Technologies Used

Python

SQLite Database

SQLAlchemy ORM

Raw SQL Queries

CLI (Command Line Interface)

# Database Design

The project consists of 4 tables:

1️. Categories

Stores expense categories like Food, Travel, Shopping, etc.

Column	Type
id	Integer (Primary Key)
name	String
2️. Expenses

Stores expense records.

Column	Type
id	Integer (Primary Key)
title	String
amount	Float
date	String (YYYY-MM-DD)
category_id	Integer (Foreign Key → categories.id)

Relationship:
One Category → Many Expenses (One-to-Many)

3️. Subscriptions

Stores recurring payments.

Column	Type
id	Integer (Primary Key)
name	String
amount	Float
next_date	String

4️. Budgets

Stores monthly spending limits.

Column	Type
id	Integer (Primary Key)
month	String (YYYY-MM)
limit	Float
# Features

Add Category

Add Expense

Update Expense

Delete Expense

Search Expense by Date

Category-wise Expense Analytics

Set Monthly Budget

Budget Exceed Alert

Persistent SQLite Storage
Learning Outcomes

This project demonstrates:

CRUD operations using ORM

One-to-Many relationship using Foreign Key

Raw SQL queries with JOIN and GROUP BY

Aggregation functions (SUM)

Parameter binding and SQL security

CLI-based modular application design

# Future Enhancements

CSV export feature

Flask-based web interface

Authentication system

Data visualization (charts)

Improved date handling using DATE type
