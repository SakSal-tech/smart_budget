# SmartBudget – Personal Finance Budget Planner

## Project Overview

SmartBudget is a web personal finance application designed to help users better understand and manage their spending habits.

Many people know their account balance but struggle to answer important questions such as:

- How much am I spending each month?
- Which categories consume most of my income?
- Am I staying within my budget?
- Am I saving enough to meet my goals?
- What changes could improve my financial wellbeing?

SmartBudget aims to provide users with simple budgeting tools and financial insights through an intuitive web application built using Python, Flask, SQL and Object-Oriented Programming principles.

---

# Problem Identification

Managing personal finances can be challenging, especially when spending is spread across multiple categories and recurring expenses.
## Why This Project?

As users of banking and budgeting apps ourselves, this is a problem we can easily relate to. Most of us may regularly manage income, expenses and savings through digital banking platforms, making it a familiar and meaningful use case. 
It also gives us the opportunity to recreate features commonly found in modern banking and FinTech applications while applying the skills learned throughout the CFG Degree.
Without a clear overview of their finances, users may:

- Overspend in certain categories
- Fail to meet savings goals
- Struggle to identify unnecessary expenses
- Lack visibility into their overall financial health

Our project addresses this problem by providing a centralised platform where users can record transactions, create budgets, track spending, and receive personalised financial feedback.

---

# Project Objectives

The primary objectives of SmartBudget are:

1. Allow users to record and manage financial transactions.
2. Enable users to create and monitor monthly budgets.
3. Categorise spending to provide meaningful insights.
4. Calculate a financial health score based on spending and savings behaviour.
5. Help users identify areas where they can improve financial management.
6. Demonstrate software engineering concepts learned throughout the CFG Degree.

---

# Core Features

## Transaction Management

Users can:

- Add transactions
- Edit transactions
- Delete transactions
- View transaction history

Must-have:

Full transaction history
Filter by income/expense
Filter by category
View by month

Nice-to-have:

Weekly summary
Daily summary
Monthly spending total

---

## Budget Management

Users can:

- Set monthly budgets
- Define spending limits by category
- Track remaining available budget
- Create monthly budget
- Set category limits
- Calculate remaining budget
- Detect overspending
- Calculate budget utilisation %

Financial Health Score
- Savings rate calculation
- Budget adherence score
- Spending behaviour score
- Overall financial health score

---

## Spending Analysis

The system will:

- Calculate total spending
- Summarise spending by category
- Identify highest spending categories
- Display budget utilisation

---

## Financial Health Score

The application will calculate a simple financial health score using factors such as:

- Savings rate
- Budget adherence
- Spending behaviour

The score will be accompanied by recommendations for improvement.

---


## Search and Filtering

Users will be able to:

- Search transactions
- Filter by category
- View spending summaries for selected categories

---

# Example of recent transactions
----------------------------------
Welcome Sarah

Monthly Budget: £2,000
Spent: £1,450
Remaining: £550

[Pie Chart]
Food 35%
Bills 30%
Travel 15%
Shopping 20%

[Line Chart]
Monthly spending trend

Recent Transactions
----------------------------------
Tesco          £45
Netflix        £10
Trainline      £18
----------------------------------


# Technology Stack

| Technology                              | Purpose |
|-----------------------------------------|---------|
| Python                                  | Core application logic |
| Flask                                   | Web application framework |
| SQL                                     | Data persistence and querying |
| Extension feature: HTML/Jinja Templates | User interface |
| GitHub                                  | Version control and collaboration |
| Jira                                    | Project management and task tracking |

---

# Software Engineering Concepts Demonstrated

| Concept | Implementation |
|----------|----------------|
| Object-Oriented Programming | User, Transaction, Budget and FinancialHealth classes |
| Data Structures | Lists and dictionaries for transaction processing and categorisation |
| Searching Algorithms | Transaction and category filtering |
| Sorting Algorithms | Ranking transactions and spending categories |
| CRUD Operations | Creating, reading, updating and deleting records |
| Database Design | Relational SQL schema |
| Version Control | GitHub workflow and pull requests |
| Agile Working | Jira task management and sprint planning |

---

# Example of Finincial Health recommendations 
You have spent 92% of your entertainment budget.

Reducing restaurant spending by £40 per month would improve your score.

Your savings rate is below your target.


# Success Criteria

The project will be considered successful if:

## Functional Requirements

- Users can create, update and delete transactions.
- Users can create and manage budgets.
- Transaction data is stored in a SQL database.
- Spending totals are calculated correctly.
- Financial health scores are generated successfully.
- Search and filtering functionality operates correctly.

## Technical Requirements

- Application is developed using Python and Flask.
- Data is persisted using SQL.
- Code follows Object-Oriented Programming principles.
- GitHub is used for collaboration and version control.
- Jira is used for project planning and task tracking.
- Code is organised, readable and documented.

## User Experience Requirements

- Interface is simple and intuitive.
- Users can navigate key features easily.
- Transaction data and Calculations are accurate
- Financial information is presented clearly.

---

# Potential Database Structure

## Users

- user_id
- name
- email

## Transactions

- transaction_id
- user_id
- amount
- category
- description
- transaction_date

## Budgets

- budget_id
- user_id
- category
- monthly_limit
- amount_spent

## Savings Goals

- goal_id
- user_id
- target_amount
- target_date

Use sample/dummy data from day one.

Even if the database is not finished, people can code using fake lists/dictionaries:

sample_transactions = [
    {"amount": 50, "category": "Groceries", "type": "expense"},
    {"amount": 2500, "category": "Salary", "type": "income"}
]

---

# Future Enhancements (Stretch Goals)

The following features may be implemented if time permits:

## Data Analytics

- Spending trend analysis
- Monthly spending reports
- Category-based summaries using Pandas

## Extension Feature if time permits: Data Visualisation?

- Spending charts
- Budget allocation graphs
- Savings progress visualisations using Matplotlib





## Suspicious Activity Detection Examples:
  - Transaction amount exceeds the user's normal spending pattern
  - Multiple transactions occur within a short period
  - Spending appears in an unusual category
  - Currency conversion or exchange rate differences create unexpected spending changes

This feature would add a risk-awareness element to the application and make the project more relevant to banking, fraud prevention and financial monitoring use cases. 
It would be implemented as a rule-based system rather than a machine learning model, keeping it realistic within the project timeframe.


## Automated Categorisation

- Automatic transaction categorisation using predefined rules

## Personalised Recommendations

- More advanced financial recommendations based on spending patterns

## Import Functionality

- Import transaction data from CSV files

## Enhanced Dashboard

- Interactive financial overview page
- Budget performance indicators
- Savings goal progress tracking

---

# Possible Task Delegation

To ensure the project is fair and collaborative, every team member will own a coding task and contribute to the GitHub repository. 
Non-coding tasks such as documentation, Jira updates, testing and presentation preparation will also be shared across the team.
This allocation is planned so there is no blocked waiting for someone else's logic.

| Team Member | Main Area                                      | Coding Contribution                                                                                                                                                                                                            |
| ----------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Person 1    | Transaction Management                         | Build Flask routes and SQL queries for creating, updating, deleting and viewing transactions, including filtering by category and transaction type                                                                             |
| Person 2    | Budget Management                              | Build Flask routes and database functionality for creating, updating, deleting and retrieving budgets and budget categories                                                                                                    |
| Person 3    | Budget Intelligence & Financial Health         | Build Python/OOP logic for remaining budget calculations, overspending detection, budget utilisation, financial health scoring and personalised recommendations                                                                |
| Person 4    | Savings Goals Management                       | Build Flask routes and SQL functionality for creating, updating, deleting and tracking savings goals and progress towards targets                                                                                              |
| Person 5    | Search, Filtering & Transaction Explorer       | Build search, filtering and sorting functionality across transactions, budgets and savings goals. Implement category searches, date-range filtering, transaction lookup, sorting by amount/date and recent activity endpoints. |
| Person 6    | Database Infrastructure, Testing & Integration | Design database schema, relationships and seed data; create unit and integration tests; maintain shared Postman collection and support feature integration                                                                     |

## Do we need Testing & Quality Lead?

    They own:
    
    - unit tests
    integration tests
    input validation tests
    reporting bugs clearly
    checking features work before merge

# Proposed Task Allocation in detail

## Team Working Principles

To ensure fair contribution across the team:

- Every team member owns a feature area.
- Every team member contributes code.
- Every team member contributes SQL queries.
- Every team member contributes tests.
- Every team member makes GitHub commits and pull requests.
- Documentation, Jira updates and presentation preparation are shared responsibilities.
- Team members can pair program and support each other when needed.

---

# Team Responsibilities

## Person 1 — Transaction Management

### Responsibilities

- Create transactions
- Edit transactions
- Delete transactions
- View transaction history
- Filter transactions by category
- Filter transactions by income/expense

### API Endpoints

```text
POST /transactions
GET /transactions
PUT /transactions/{id}
DELETE /transactions/{id}
```

### Technical Skills Demonstrated

- Flask routes
- CRUD operations
- SQL queries
- Validation
- Error handling

---

## Person 2 — Budget Management

### Responsibilities

- Create budgets
- Update budget limits
- Delete budgets
- Retrieve budgets
- Manage budget categories

### API Endpoints

```text
POST /budgets
GET /budgets
PUT /budgets/{id}
DELETE /budgets/{id}
```

### Technical Skills Demonstrated

- Flask routes
- CRUD operations
- SQL queries
- Validation
- Database interaction

### Notes

This role is responsible for storing and managing budget data.
Budget calculations are handled by Person 3.

---

## Person 3 — Budget Intelligence & Financial Health

### Responsibilities

#### Budget Calculations

- Calculate remaining budget
- Calculate budget utilisation percentage
- Detect overspending
- Compare spending against budget limits

#### Financial Health Score

- Calculate savings rate
- Calculate budget adherence score
- Generate financial health score

#### Recommendations Engine

- Generate personalised recommendations
- Generate overspending alerts
- Generate financial wellbeing insights

### API Endpoints

```text
GET /budget-summary
GET /health-score
GET /recommendations
```

### Technical Skills Demonstrated

- OOP
- Algorithms
- Data structures
- Business logic
- Calculations
- Financial modelling

### Example Outputs

```text
Remaining Budget: £450

Health Score: 82/100

You have spent 92% of your entertainment budget.

Increasing monthly savings by £50 would improve your financial health score.
```

---

## Person 4 — Savings Goals Management

### Responsibilities

- Create savings goals
- Update savings goals
- Delete savings goals
- Track progress towards goals
- Calculate percentage completion

### API Endpoints

```text
POST /savings-goals
GET /savings-goals
PUT /savings-goals/{id}
DELETE /savings-goals/{id}
```

### Technical Skills Demonstrated

- CRUD operations
- Flask routes
- SQL queries
- Validation
- OOP

---

## Person 5 — Search, Filtering & Transaction Explorer

### Responsibilities

* Search transactions by category
* Search transactions by date range
* Search budgets by category
* Search savings goals
* Filter income vs expenses
* Sort transactions by amount
* Sort transactions by date
* View recent transactions
* View largest transactions

### API Endpoints

```text
GET /transactions/search
GET /transactions/filter
GET /transactions/sort
GET /transactions/recent
GET /transactions/largest
GET /budgets/search
GET /savings-goals/search
```

### Technical Skills Demonstrated

```text
Flask routes
Search algorithms
Sorting algorithms
SQL queries
JOIN queries
Filtering logic
Data structures
API endpoint design
```

### Optional Stretch Goals

```text
Advanced multi-criteria filtering
Search performance optimisation
Pagination for large transaction histories
Most-used spending categories
Recently viewed searches
```

---

## Person 6 — Database Infrastructure, Testing & Integration

### Database Responsibilities

- Design database schema
- Define relationships between tables
- Create seed/sample data
- Support complex JOIN queries
- Maintain shared database setup scripts

### Testing Responsibilities

- Unit tests
- Integration tests
- API validation tests
- Shared Postman collection

### Integration Responsibilities

- Verify application works after merges
- Support integration testing
- Assist with merge conflict resolution
- Verify endpoint consistency

### Technical Skills Demonstrated

- SQL database design
- Relational modelling
- Testing
- Validation
- Git collaboration
- Integration support

---

# Shared Responsibilities

All team members contribute to:

- GitHub commits
- Pull requests
- Code reviews
- Jira updates
- Project activity logs
- README documentation
- Presentation slides
- Demo preparation

---

# Git Workflow

## Branches

```text
main
dev
feature/*
```

### main

Stable version of the application.

### dev

Shared integration branch used to combine completed features before release.

### feature branches

Examples:

```text
feature-transactions
feature-budgets
feature-budget-intelligence
feature-savings-goals
feature-reporting
feature-testing
```

---

## Merge Process

1. Develop feature on feature branch
2. Push feature branch to GitHub
3. Create Pull Request into dev
4. Resolve conflicts if required
5. Test integrated functionality in dev
6. Merge dev into main when stable

---

# Definition of Done

A task is considered complete when:

- Functionality works locally
- Relevant tests pass
- Code is committed to GitHub
- Pull Request has been created
- Jira ticket has been updated
- Documentation has been updated where necessary

## Shared Responsibilities

All team members will also contribute to:

- GitHub commits and pull requests
- Jira task updates
- debugging their own code
- Code reviews
- Project activity log
- Documentation
- Presentation preparation
- Final demo practice

## Collaboration Agreement

Each person should own at least one feature, but team members can pair up if anyone gets stuck. If someone is struggling or unavailable, they should let the group know early so the team can adjust tasks and keep the project on track.


## External API Integration https://frankfurter.dev/

SmartBudget will integrate with a currency exchange rate API to support international spending and travel-related transactions. Users will be able to record purchases made abroad and view their value in their home currency, helping them better understand the true impact of holiday and overseas spending on their budget.

This feature also provides insight into how currency fluctuations can affect spending power, savings goals and financial planning. It reflects functionality commonly found in modern banking and FinTech applications, making the project both practical and relevant to everyday users.


## Deligation Difficulty & Time Consumption

| Rank | Team Member  | Main Area                                      | Difficulty      | Time Consumption | Why                                                                                                                               |
| ---- | ------------ | ---------------------------------------------- | --------------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| 1    | **Person 4** | Savings Goals Management                       | ⭐ Easy          | ⭐⭐ Low–Medium    | Mostly CRUD operations and progress tracking. Straightforward Flask routes and SQL queries.                                       |
| 2    | **Person 2** | Budget Management                              | ⭐⭐ Easy–Medium  | ⭐⭐ Medium        | CRUD for budgets and categories with some validation and database relationships.                                                  |
| 3    | **Person 1** | Transaction Management                         | ⭐⭐⭐ Medium      | ⭐⭐⭐ Medium–High  | Core feature of the application. More routes, validation, filtering and transaction handling.                                     |
| 4    | **Person 5** | Search, Filtering & Transaction Explorer       | ⭐⭐⭐ Medium–High | ⭐⭐⭐ Medium–High  | Requires search and sorting logic, filtering, SQL queries, joins and specialist-topic implementation.                             |
| 5    | **Person 6** | Database Infrastructure, Testing & Integration | ⭐⭐⭐⭐ High       | ⭐⭐⭐⭐ High        | Designs schema, manages relationships, creates tests, supports integration and helps resolve issues across the project.           |
| 6    | **Person 3** | Budget Intelligence & Financial Health         | ⭐⭐⭐⭐⭐ Very High | ⭐⭐⭐⭐⭐ Very High  | Most algorithmic role. Requires OOP design, calculations, financial health scoring, recommendations and business logic decisions. |
