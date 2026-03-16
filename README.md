# -AI-Natural-Language-SQL-Agent
An AI-powered system that converts natural language questions into SQL queries  using Google Gemini and executes them on a Supabase PostgreSQL database  through n8n workflow automation.
# AI Natural Language Database Query System

This project allows users to retrieve data from a database using natural language questions.

The system converts user questions into SQL queries using AI and executes them automatically on a Supabase PostgreSQL database.
The user only receives the final result data, not the SQL query.

---

# Project Overview

This system integrates AI with workflow automation to allow database access using simple human language.

Instead of writing SQL manually, users can ask questions like:

Show all customers
Show freight cost data
List forecast monthly records
Show gross price details

The system processes the question and returns the result directly from the database.

---

# Technologies Used

* n8n – workflow automation
* Google Gemini – natural language understanding
* PostgreSQL – relational database
* Supabase – database hosting platform

---

# System Architecture

User Question
↓
n8n Chat Trigger
↓
AI Agent (Gemini)
↓
Convert Question → SQL Query
↓
Execute Query in Supabase Database
↓
Fetch Data from Tables
↓
Return Result Only to the User

---

# Example Usage

User Input

Show all customers

System Output

Customer table data displayed to the user.

---

User Input

Show freight cost data

System Output

Freight cost table records returned.

---

User Input

Show forecast monthly data

System Output

Forecast monthly data returned from the database.

---

# Database Tables

The database hosted on Supabase contains multiple tables such as:

customer
fact_forecast_monthly
fact_freight_cost
fact_gross_price

The AI agent dynamically retrieves information from these tables.

---

# Workflow Links

Main Workflow

![https://n8n.io/workflows/](https://github.com/srinathnporange/-AI-Natural-Language-SQL-Agent/blob/main/6179236450705018332.jpg)

SQL Execution Workflow

![https://n8n.io/workflows/](https://github.com/srinathnporange/-AI-Natural-Language-SQL-Agent/blob/main/6179236450705018334.jpg)

*(Replace with your workflow export or public workflow links)*

---

# Database Link


Database Tables

![database](https://github.com/srinathnporange/-AI-Natural-Language-SQL-Agent/blob/main/6179236450705018340.jpg)

---

# Project Structure

ai-natural-language-sql-agent

README.md
workflows/
 ai-agent-workflow.json
 execute-sql-query.json

database/
 schema.sql

screenshots/
 workflow.png
 supabase_tables.png
 execution_result.png

docs/
 architecture.md

---


# Output

The system processes the question and returns database results directly to the user.

No SQL query is displayed to the user.

---

# Future Improvements

Add web interface for users
Add authentication layer
Add query safety validation
Support complex analytical queries

---
