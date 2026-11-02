# Bank Loan Eligibility System

A Python-based loan eligibility application designed to evaluate customer information, calculate annual income, and assess loan applications against predefined eligibility criteria.

Built as a practical Python project, it demonstrates how fundamental programming concepts can be applied to a banking-related scenario, combining input validation, financial calculations, and conditional decision-making.

---

## Overview

The Bank Loan Eligibility System is a command-line application that simulates a basic bank loan eligibility assessment.

The program collects customer information, including name, age, monthly income, account balance, and existing pending loan amount.

It validates the customer's name and age, calculates annual income, and evaluates the application against predefined banking criteria.

Based on the provided information, the system identifies eligibility issues and displays the corresponding messages. Customers who satisfy all the implemented conditions receive an eligibility confirmation.

## Features

- Customer name validation
- Age input validation
- Monthly income assessment
- Account balance information collection
- Automatic annual income calculation
- Existing pending loan evaluation
- Multiple eligibility condition checks
- Clear rejection messages for unmet criteria
- Conditional loan eligibility confirmation
- Console-based report output

---

## Loan Eligibility Criteria

The application evaluates loan eligibility using predefined conditions.

### 1. Customer Age

Customers must meet the minimum age requirement.

| Age | Condition |
|---|---|
| Below 1 | Invalid age |
| 1–17 | Not eligible for a loan |
| 18–95 | Meets age requirement |
| Above 95 | Invalid age |

### 2. Monthly Income

The minimum monthly income requirement is Rs. 30,000.

| Monthly Income | Eligibility |
|---|---|
| Rs. 30,000 or above | Meets income requirement |
| Below Rs. 30,000 | Does not meet income requirement |

### 3. Existing Pending Loan

The application checks the customer's existing pending loan amount.

| Pending Loan Amount | Eligibility |
|---|---|
| Below Rs. 500,000 | Meets loan requirement |
| Rs. 500,000 or above | Does not meet loan requirement |

### 4. Annual Income Calculation

Annual income is calculated by multiplying the monthly income by 12.

**Formula:**

Annual Income = Monthly Income × 12

The calculated annual income is displayed in the program output.

---

## Eligibility Assessment

The application initializes the eligibility status as `True` and checks each condition separately.

If any of the following conditions are not met, eligibility is changed to `False`:

- Monthly income is below Rs. 30,000.
- Customer age is below 18.
- Existing pending loan amount is Rs. 500,000 or above.

A loan eligibility confirmation is displayed only when all implemented conditions are satisfied.

---

## Technologies & Concepts

**Programming Language:** Python 3

**Core Concepts Used:**

- Variables and data types
- User input using `input()`
- Type conversion using `int()`
- String methods (`.replace()`, `.isalpha()`)
- While loops for input validation
- Conditional statements (`if`, `else`)
- Multiple independent conditional checks
- Boolean variables (`True`, `False`)
- Arithmetic operations
- Comparison and logical operators
- Decision-making and control flow
- Console-based output formatting

No external Python libraries are required.

---

## Sample Run

### Customer Input

```text
"BANK ELIGIBILITY REPORT"

What is your Name Sir ? Ahmed Khan
What is your Age ? 30
Enter your Current Monthly Income = 56000
Enter your Current Account Balance = 45600
Enter your Existing Pending Loan Amount = 23000
```

### Generated Output

```text
Annual Income = 672000
Congratulations, you are eligible for our bank loan.
```

### Example: Eligibility Rejection

```text
"BANK ELIGIBILITY REPORT"

What is your Name Sir ? RJ
What is your Age ? 13
Enter your Current Monthly Income = 56000
Enter your Current Account Balance = 45600
Enter your Existing Pending Loan Amount = 23000

Annual Income = 672000
Sorry, your age must be at least 18.
```

The second example demonstrates how an applicant can meet the financial criteria but fail the minimum age requirement.

---

## Getting Started

### Requirements

- Python 3
- A code editor or Python-compatible IDE
- No additional package installation required

### Installation & Execution

**1. Clone the repository**

```bash
git clone https://github.com/your-username/BANK-LOAN-ELIGIBILITY-SYSTEM.git
```

**2. Navigate to the project directory**

```bash
cd BANK-LOAN-ELIGIBILITY-SYSTEM
```

**3. Run the Python application**

```bash
python loan_eligibility_system.py
```

Follow the on-screen prompts to enter customer information and financial details.

---

## Project Structure

```text
BANK-LOAN-ELIGIBILITY-SYSTEM/
│
├── loan_eligibility_system.py
├── README.md
└── LICENSE
```

An optional Jupyter Notebook version can also be included:

```text
BANK-LOAN-ELIGIBILITY-SYSTEM/
│
├── loan_eligibility_system.py
├── BANK_LOAN_ELIGIBILITY_SYSTEM.ipynb
├── README.md
└── LICENSE
```

---

## Learning Objectives

This project provides practical experience in applying Python fundamentals to a banking-related eligibility assessment scenario.

The main focus is on:

- Validating user information through string methods
- Using while loops to handle incorrect input
- Understanding the difference between input validation and eligibility assessment
- Calculating annual income using arithmetic operations
- Applying multiple independent eligibility conditions
- Working with Boolean variables and conditional logic
- Evaluating different application outcomes
- Translating predefined business rules into Python code

---

## Future Improvements

Potential enhancements to the application include:

- Adding validation for negative income, account balance, and loan amounts
- Including account balance in the eligibility assessment
- Introducing additional loan qualification criteria
- Calculating loan affordability based on monthly income
- Generating a detailed loan eligibility report
- Adding application reference numbers
- Maintaining customer application records
- Improving the final eligibility summary

---

## Author

**Rammal Ahmed**

AI & Data Science Enthusiast | Microsoft Dynamics 365 CRM Developer | Power Platform | UI/UX Designer | Graphic Designer & Illustrator

[LinkedIn] www.linkedin.com/in/rammal-ahmed-58184b325 · [GitHub] https://github.com/Rammal-Ahmed

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

**Project Status:** Completed
