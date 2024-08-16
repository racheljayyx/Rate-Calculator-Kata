# Rate-Calculator-Kata

## Overview

This is a technical test kata completed for practice. The goal is to implement a rate calculation system that allows prospective borrowers to obtain a quote from a pool of lenders for 36-month loans. The system will be implemented as a command-line application.

## Specifications

### Input Data

You will be provided with a CSV file containing a list of all the offers made by lenders within the system. An example of this file is provided as `market.csv`.

### Key Requirements

- **Loan Amount**: Borrowers can request a loan in increments of £100, ranging from £1,000 to £15,000 inclusive.
- **Optimal Rate**: The system should aim to offer the lowest possible rate to ensure competitive quotes.
- **Output Details**: The borrower should receive the following details:
  - **Rate**: The interest rate for the loan, displayed to one decimal place.
  - **Monthly Repayment**: The monthly repayment amount, displayed to two decimal places.
  - **Total Repayment**: The total repayment amount, displayed to two decimal places.

### Insufficient Offers

If there are not enough offers from lenders to fulfill the requested loan amount, the system should inform the borrower that it is not possible to provide a quote at that time.

## Command-Line Interface

The application should be executed with the following arguments:
```
cmd> [application] [market_file] [loan_amount]    
```
Example: 
```
cmd> quote.exe market.csv 1500
```


The application should produce output in the form: 
```
cmd> [application] [market_file] [loan_amount]
Requested amount: £1500
Rate: X.X%
Monthly repayment: £XXX.XX
Total repayment: £XXXX.XX
```
Example: 
```
cmd> quote.exe market.csv 1000
Requested amount: £1000
Rate: 7.0%
Monthly repayment: £30.78
Total repayment: £1108.10
```

## Remaarks
- We do not mind what language you chose for your implementation 
- The monthly and total repayment should use monthly compounding interest 
- We will review your code and run it against some other test cases to see how it handles them 

