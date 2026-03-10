Monday.com Business Intelligence Agent

This project implements an AI-powered Business Intelligence Agent that answers founder-level business queries by integrating with Monday.com boards containing Deals (pipeline data) and Work Orders (execution data).

The agent retrieves board data using the Monday.com API, cleans inconsistent real-world data, and provides insights about pipeline health, sector performance, and operational metrics through a conversational query interface.

Features

Integration with Monday.com API

Handles messy real-world business data

Supports conversational business queries

Generates leadership-level insights

Works across multiple boards (Deals + Work Orders)

Data Sources

The agent reads data from two Monday.com boards:

Deal Funnel Board

Sales pipeline data

Deal value

Sector

Deal stage

Close dates

Work Order Tracker Board

Project execution data

Work order status

Execution timeline

Operational workload

Example Queries

The agent can answer queries such as:

How is our pipeline looking?
What is the total pipeline value?
Show pipeline by sector
Which sector has the highest deal value?
Show work orders summary
How many active work orders are there?
Generate leadership update
Example Output
Leadership Update

Total Pipeline Value: 1,042,673,427

Work Orders
Active: 3
Completed: 83

Insight:
Current pipeline indicates strong deal flow with manageable operational workload.
Tech Stack

Python

Pandas

Requests

Monday.com GraphQL API

Google Colab (development environment)

Architecture
User Query
     ↓
Query Processing Agent
     ↓
Monday.com API
     ↓
Data Cleaning & Processing
     ↓
Business Intelligence Insights
Data Resilience Handling

The agent handles messy real-world data by:

Filling missing values

Converting inconsistent numeric fields

Handling incomplete records gracefully

Providing meaningful insights even with partial data

Future Improvements

Natural language query understanding using LLMs

Dashboard visualization

Predictive pipeline forecasting

Automated weekly leadership reports
