# Jira Cloud API Automation Framework

## Overview

This project demonstrates End-to-End REST API Automation for Jira Cloud using Postman and Newman. It automates the complete issue lifecycle by retrieving project details, fetching issue types, creating issues dynamically using CSV data, validating responses, retrieving created issues, and assigning them to a user.

The framework follows a Data-Driven Testing approach, allowing multiple issue types to be tested without modifying the API requests.

---

## Tech Stack

- Postman
- Newman
- Jira Cloud REST API
- JavaScript
- CSV Data-Driven Testing
- JSON
- Git
- GitHub

---

## Features

- Get Project Details
- Get Issue Types for a Project
- Get Assignable User
- Create Issues Dynamically
- Retrieve Created Issue
- Assign Issue
- Response Validation
- Collection Variables
- Environment Variables
- Data-Driven Testing using CSV
- Newman CLI Execution

---

## Project Flow

1. Get Project Details
2. Get Issue Types
3. Get Assignable User
4. Read Test Data from CSV
5. Create Issue
6. Validate Response
7. Retrieve Created Issue
8. Assign Issue
9. Validate Assignment

---

## Test Data

csv
IssueName,issueSummary
Story,DataDrivenTesting- Issue Type Story
Bug,DataDrivenTesting- Issue Type Bug
Task,DataDrivenTesting- Issue Type Task


---

## Project Structure


Jira_API_Automation/
│
├── API Test Jira Cloud.postman_collection.json
├── Jira Environment.postman_environment.json
├── csv_testdata.csv
├── README.md


---

## Running the Project

Run the collection using Newman:

bash
newman run "API Test Jira Cloud.postman_collection.json" \
-e "Jira Environment.postman_environment.json" \
-d "csv_testdata.csv"


---

## Sample Execution Result

- Iterations: 3
- Requests: 18
- Assertions: 6
- Failed: 0

---

## Learning Highlights

- REST API Testing
- Postman Scripting
- Newman CLI
- JavaScript
- JSON Parsing
- Dynamic Variable Handling
- Collection Variables
- Environment Variables
- Data-Driven Testing
- Response Validation
- End-to-End API Automation

---

## Challenges Solved

- Handled Internet Connectivity (ECONNRESET) issues.
- Dynamically extracted Issue Type ID.
- Replaced map() + indexOf() with find() for cleaner object lookup.
- Fixed JavaScript syntax issues during debugging.
- Resolved an extra Newman iteration caused by an improperly formatted CSV file.
- Created a clean UTF-8 CSV using Notepad to ensure reliable Data-Driven execution.

---

## Future Enhancements

- HTML Reporting
- GitHub Actions CI/CD
- Multiple Environment Support
- Negative Test Scenarios
- API Chaining Enhancements

---

## Author

*Reetika Srivastava*

QA Automation Engineer

### Skills

- Manual Testing
- API Testing
- Postman
- Newman
- Jira
- Selenium (Learning)
- Python
- Git & GitHub

  <img width="767" height="858" alt="Data Driven Test Added" src="https://github.com/user-attachments/assets/d4da4865-a654-41d0-b0af-2c9542cbba24" />
<img width="1510" height="972" alt="Newman" src="https://github.com/user-attachments/assets/6758b5c2-a66e-4370-9ce9-09879ceafc1f" />

