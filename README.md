# Loan Eligibility System

A small collection of beginner-friendly JavaScript programs demonstrating conditional logic, user input, and financial decision-making. The main example evaluates a loan application using income, monthly EMI, and credit score; the folder also includes an e-commerce order calculation example.

> **Note:** The loan result is an educational example based on simple rules. It is not a real lending decision or financial advice.

## What’s inside

| File | Description |
| --- | --- |
| `loan.js` | Prompts for applicant details and prints a loan eligibility report. |
| `2ndindex.js` | Another copy of the loan eligibility example. |
| `ecommerce.js` | Calculates an order discount, delivery charge, and final payable amount. |
| `index.js` | Another copy of the e-commerce example. |

## Requirements

- [Node.js](https://nodejs.org/) installed on your computer
- A terminal or command prompt

No additional packages are required; the loan program uses Node.js’s built-in `readline` module.

## Run the loan example

Open a terminal in the project folder and run:

```bash
node loan.js
```

Enter the requested values when prompted:

1. Monthly income
2. Loan amount
3. Monthly EMI
4. Credit score

The program checks that income and loan amount are positive, EMI is non-negative, and credit score is between 300 and 900. It then displays one of these outcomes:

- **GREEN SIGNAL — Standard Applicant:** credit score is at least 750 and EMI is no more than 40% of monthly income.
- **NEEDS REVIEW — Conditional Applicant:** credit score is at least 650 and EMI is no more than 50% of monthly income.
- **RED SIGNAL — High-Risk Applicant:** the application does not meet either threshold.
- **INVALID APPLICATION:** one or more entered values are outside the accepted input range.

For example, an applicant with a monthly income of ₹50,000, an EMI of ₹18,000, and a credit score of 760 receives a **GREEN SIGNAL**. The loan amount must also be greater than zero.

## Run the e-commerce example

```bash
node ecommerce.js
```

This example uses sample values defined in the source file. It applies a membership discount, adds an extra discount for orders above ₹5,000, caps the total discount at 20% of the order amount, and calculates delivery charges. Update the values near the top of `ecommerce.js` to try different scenarios.

## Project status

These are standalone learning exercises. The loan example uses fixed eligibility thresholds and does not connect to a lender, store application data, or validate whether every entry is a numeric value.
