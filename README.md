# Mortgage Calculator

## Task overview

Create a web application where users can create banks and calculate mortgage payments using one of these bank’s settings.

## Tasks

* [Banks management page](#banks-management-page)
* [Mortgage calculator page](#mortgage-calculator-page)

### Banks management page
On this page, a user should be able to see the list of all earlier created banks and create/edit/remove the bank.

Here is the example of bank schema that might be convenient to use during the development:

* Bank name

* Interest rate - the annual percentage rate that expresses the amount of money the bank charges additionally for the use of assets the person borrowed money for.

* Maximum loan - the maximum amount of money a bank is able to borrow.

* Minimum down payment - the amount of money a person needs to pay upfront (if a person takes a loan of $300.000 and bank minimum down payment is 20%, it means that person must pay the bank $60.000 as an initial mortgage payment)

* Loan term - a period of time in which a person must pay off the loan.

### Mortgage calculator page
Here the user can see the payment plan for his mortgage.

This page should contain the following inputs:

* Initial loan (example: $280.000)

* Down payment (example: $20.000)

* Bank (enter the name or select from dropdown)

Based on entered data you can apply the next formula to calculate monthly mortgage payment:

$$ M = {P({r \over 12})(1+{r \over 12})^n \over (1+{r \over 12})^n - 1} $$

* M = mountly payment

* P = amount borrowed

* r = annual interest rate

* n = number of mounthly payments

User’s entered data should be validated according to the selected bank, for example down payment satisfies the minimum down payment boundary of the bank,  the bank is capable of giving a requested loan.