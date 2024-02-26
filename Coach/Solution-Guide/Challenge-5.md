# Challenge 5: Create Documentation using GitHub Copilot - Solution Guide

## Task 1: Generate Documentation with Copilot

In this task, you'll utilize GitHub Copilot to generate comments and markdown documentation for a selected piece of code.

1. Open Visual Studio Code and copy the below python code in a new file.

   > **Note:** This code defines classes for a bank account and a customer, demonstrating basic banking operations like deposit, withdrawal, and checking the balance. It also creates two customers with their respective accounts and performs some transactions.

   ```
    class BankAccount:
      def __init__(self, account_holder, balance=0):
            self.account_holder = account_holder
            self.balance = balance

        def deposit(self, amount):
            if amount > 0:
                self.balance += amount
                print(f"Deposited ${amount}. New balance: ${self.balance}")
            else:
                print("Invalid deposit amount.")

        def withdraw(self, amount):
            if 0 < amount <= self.balance:
                self.balance -= amount
                print(f"Withdrew ${amount}. New balance: ${self.balance}")
            else:
                print("Invalid withdrawal amount or insufficient funds.")

        def check_balance(self):
            print(f"Current balance for {self.account_holder}: ${self.balance}")

    class Customer:
        def __init__(self, name):
            self.name = name
            self.accounts = []

        def add_account(self, account):
            self.accounts.append(account)
            print(f"Added account for {self.name}")

    def main():
        customer1 = Customer("Alice")
        customer2 = Customer("Bob")

        account1 = BankAccount("Checking", 1000)
        account2 = BankAccount("Savings", 500)

        customer1.add_account(account1)
        customer2.add_account(account2)

        account1.deposit(200)
        account2.withdraw(100)

        account1.check_balance()
        account2.check_balance()

    if __name__ == "__main__":
        main()
   ```

1. Select the entire code, right click and select **Copilot** and **Generate Docs**.

1. You'll notice that GitHub Copilot has generated comments for the class **BankAccount**.

   ```
   """
   A class representing a bank account.

   Attributes:
   - account_holder (str): The name of the account holder.
   - balance (float): The current balance of the account.

   Methods:
   - deposit(amount): Deposits the specified amount into the account.
   - withdraw(amount): Withdraws the specified amount from the account.
   - check_balance(): Prints the current balance of the account.
   """
   ```

1. To generate a markdown documentation for the above code, select the entire code, right click and select **Copilot** and **Start Inline Chat** and ask the GitHub Copilot to generate a markdown documentation for the selected code.

1. You'll notice that GitHub Copilot has generated a Markdown documentation specifically for the selected code.

   ```
   """
   # Bank Account System

   ## BankAccount Class

   A class representing a bank account.

   ### Attributes:
   - `account_holder` (str): The name of the account holder.
   - `balance` (float): The current balance of the account.

   ### Methods:
   - `deposit(amount)`: Deposits the specified amount into the account.
   - `withdraw(amount)`: Withdraws the specified amount from the account.
   - `check_balance()`: Prints the current balance of the account.

   ## Customer Class

   A class representing a customer.

   ### Attributes:
   - `name` (str): The name of the customer.
   - `accounts` (list): A list of bank accounts associated with the customer.

   ### Methods:
   - `add_account(account)`: Adds a bank account to the customer's list of accounts.

   ## Main Function

   The main function creates two customers, each with their own bank account. It performs some operations on the accounts, such as depositing and withdrawing money, and then checks the balances.

   To run the program, execute the `main()` function.
   ```

## Task 2: Customize and Refine Documentation

In this task, you'll customize and refine your documentation process by utilizing GitHub Copilot Inline Chat, Suggestions and Explain feature.

1. Select the entire code (from the above task), right click and select **Copilot** and **Start Inline Chat**. Ask the GitHub Copilot to generate descriptive comments for the selected code.

1. You'll notice that the GitHub Copilot has generated descriptive comments for each class, definition and function.

1. You can also enhance the documentation and the code through GitHub Copilot's Suggestion window. Select the code and click **Ctrl+Enter** to view Suggestions provided by GitHub Copilot to refine the document or code.

1. You'll find a number of suggestions for the selected document or code which will enhance and refine the same.

1. To get more elaborated explanation about any code, select the code, right click and select **Copilot** and **Explain This**.

1. You'll notice in the GitHub Copilot Chat window, provides a detailed and clear explanation of the code.




















