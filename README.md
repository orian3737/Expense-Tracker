# Finance Tracker

## Description

Finance Tracker is a Python-based CLI application that helps users manage their financial transactions. Users can log income and expenses, view a summary within a date range, and visualize their financial data with interactive plots.

## Features

- Add new transactions with details such as date, amount, category, and description.
- Retrieve and summarize transactions within a specific date range.
- Visualize income and expenses over time using line plots.
- Interactive prompts for data entry with validation.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/orian3737/Expense-Tracker.git
   cd Expense-Tracker
   ```

2. Create a virtual environment:

- Check your Python version: Ensure Python 3.11 is installed on your system:

   ```bash
   python --version
   ```

- If it shows a version lower than 3.11, update your Python installation.
Set up a pip environment: Ensure you have pip installed and updated:

   ```bash
   pip install --upgrade pip
   ```

3. Install dependencies:

   ```bash
    pip install pandas matplotlib
    pip list
   ```

## Usage

1. Initialize the application by running:

   ```bash
   python app.py
   ```

2. Follow the interactive prompts to:

   ```bash
   Add a new transaction.
   View transactions within a specific date range.
   Plot income and expenses.
   Exit the application by selecting the appropriate option in the menu.
   ```

## Project Structure

   ```bash
   .
   ├── app.py                # Main application entry point
   ├── data_entry.py         # Helper functions for data input
   ├── finance_data.csv      # CSV file to store transaction data
   ├── requirements.txt      # Python dependencies
   ├── README.md             # Project documentation
   ```

## Dependencies

The project uses the following libraries:

- pandas for data manipulation.
- matplotlib for data visualization.

All dependencies are specified in requirements.txt.

## Functionality

### Adding Transactions

- Users can enter a transaction with the following details:
- Date: In dd-mm-yyyy format (defaults to today's date if left blank).
 -Amount: A positive float value.
 -Category: Income or Expense.
 -Description: Optional text.

### Viewing Transactions

- Retrieve transactions between two dates.
- Displays a summary:
- Total income.
- Total expense.
- Net savings.

### Plotting Transactions

- Visualize income and expenses over time with an interactive line plot.
![Capture](https://github.com/user-attachments/assets/6f11ff61-1c98-4b76-888c-f984f8ed921f)

### Example Usage

1. Adding a Transaction:

   ```bash
   1. Enter the date of the transaction (dd-mm-yyyy) or enter for today's date: 21-11-2024
   2. Enter the amount: 150.50
   3. Enter the category ('I' for Income or 'E' for Expense): I
   4. Enter a description (optional): Freelance Work
   5. Entry added successfully.
   ```

2. Viewing Transactions:

     ```bash
     Enter the start date (dd-mm-yyyy): 01-11-2024
     Enter the end date (dd-mm-yyyy): 21-11-2024
     Transactions from 01-11-2024 to 21-11-2024:
     date        amount   category   description
     01-11-2024    150.50   Income     Freelance Work

     Summary:
     Total income: $150.50
     Total expense: $0.00
     Net savings: $150.50
     ```

3. Plotting Data:

- After viewing transactions, users can opt to generate a plot of income and expenses over time.

### License

This project is licensed under the MIT License. See the LICENSE file for details.

### Contributing

1. Fork the repository.
2. Create a new branch (git checkout -b feature-name).
3. Commit your changes (git commit -m "Add feature").
4. Push to the branch (git push origin feature-name).
5. Create a pull request.

### Author

Developed by Ryan Murzyn. Contributions and feedback are welcome!
