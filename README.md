# Personal Finance Tracker

A simple Python app to track your income and expenses. Nothing fancy, just basic stuff to help you keep track of your money.

## What's in here?

### `main.py`
This is the main file you run to start the app. It does:
- Shows you a menu with 3 options: add transaction, view transactions, or exit
- Handles adding new income/expense entries to your CSV file
- Lets you view transactions between any two dates
- Shows you a summary (total income, total expense, net savings)
- Can plot a graph showing your income vs expenses over time (if you want)

### `data_entry.py`
This file handles all the user inputs. It has functions to:
- Get and validate dates (makes sure you enter them in dd-mm-yyyy format)
- Get amount (makes sure it's a valid positive number)
- Get category (Income or Expense - you just type 'I' or 'E')
- Get description (optional text about the transaction)

Basically, this file makes sure you don't mess up when entering data.

### `finance_data.csv`
This is where all your transaction data gets saved. It has 4 columns:
- date (when the transaction happened)
- amount (how much money)
- category (Income or Expense)
- description (what it was for)

The app creates this file automatically if it doesn't exist.

### `requirements.txt`
Just lists the libraries you need to install:
- `pandas` - for handling the data
- `matplotlib` - for making the graphs

## How to use

1. Install the requirements: `pip install -r requirements.txt`
2. Run the app: `python main.py`
3. Follow the prompts to add transactions or view your financial data

That's it! Pretty straightforward.