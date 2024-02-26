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

## Task 3: Explore Various Documentation Styles

In this task, you'll explore on various styles of documentation that you can generated by utilizing GitHub Copilot.

1. In your VS Code, create a new file, right click anywhere on the new file and select **Copilot** and **Start Inline Chat**.

1. Ask the GitHub Copilot to generate a markdown docmentation to deploy a VNet in Azure and click **Accept**.

1. You'll notice that the GitHub Copilot has generated a step by step markdown documentation to deploy a VNet in Azure.

   ```
   # Deploy a Virtual Network (VNet) in Azure

   ## Introduction
   In this guide, we will walk you through the steps to deploy a Virtual Network (VNet) in Azure. A VNet is a fundamental building block for any Azure infrastructure deployment, as it provides isolation and segmentation of resources.

   ## Prerequisites
   Before you begin, make sure you have the following:
   - An Azure subscription
   - Sufficient permissions to create resources in Azure
   
   ## Steps

   ### 1. Sign in to the Azure portal
   - Open a web browser and navigate to the [Azure portal](https://portal.azure.com).
   - Sign in with your Azure account.

   ### 2. Create a new Virtual Network
   - In the Azure portal, click on the **Create a resource** button.
   - Search for "Virtual Network" and select **Virtual Network** from the search results.
   - Click on the **Create** button to start the creation process.

   ### 3. Configure the Virtual Network
   - Provide a **Name** for the Virtual Network.
   - Select the appropriate **Subscription**.
   - Choose a **Resource group** or create a new one.
   - Select the **Region** where you want to deploy the Virtual Network.
   - Configure the **Address space** for the Virtual Network.
   - Optionally, configure the **Subnets** within the Virtual Network.
   - Click on the **Review + create** button to proceed.

   ### 4. Review and create the Virtual Network
   - Review the configuration settings for the Virtual Network.
   - Click on the **Create** button to start the deployment process.
   
   ### 5. Monitor the deployment
   - Once the deployment is initiated, you can monitor the progress in the Azure portal.
   - Wait for the deployment to complete.

   ## Conclusion
   Congratulations! You have successfully deployed a Virtual Network in Azure. You can now start using the Virtual Network to host your    Azure resources.

   ## Next Steps
   - Connect the Virtual Network to other Azure resources.
   - Configure network security and routing within the Virtual Network.
   - Explore advanced networking features in Azure.
   ```

1. You can also utilize GitHub Copilot to generate a Javadoc to create a calculator.

   ```
   /**
    * This class represents a calculator that can perform basic arithmetic operations.
    */
   public class Calculator {
    
       /**
        * Adds two numbers and returns the result.
        *
        * @param num1 The first number.
        * @param num2 The second number.
        * @return The sum of the two numbers.
        */
       public int add(int num1, int num2) {
           return num1 + num2;
       }
    
       /**
        * Subtracts two numbers and returns the result.
        *
        * @param num1 The first number.
        * @param num2 The second number.
        * @return The difference between the two numbers.
        */
       public int subtract(int num1, int num2) {
           return num1 - num2;
       }
    
       /**
        * Multiplies two numbers and returns the result.
        *
        * @param num1 The first number.
        * @param num2 The second number.
        * @return The product of the two numbers.
        */
       public int multiply(int num1, int num2) {
           return num1 * num2;
       }
    
       /**
        * Divides two numbers and returns the result.
        *
        * @param num1 The first number.
        * @param num2 The second number.
        * @return The quotient of the two numbers.
        * @throws ArithmeticException if the second number is zero.
        */
       public double divide(int num1, int num2) {
           if (num2 == 0) {
               throw new ArithmeticException("Cannot divide by zero");
           }
           return (double) num1 / num2;
       }
   }
   /**
    * Performs multiplication for three variables or numbers.
    *
    * @param a The first number.
    * @param b The second number.
    * @param c The third number.
    * @return The result of multiplying the three numbers.
    */
   public int multiply(int a, int b, int c) {
       return a * b * c;
   }
   ```


















