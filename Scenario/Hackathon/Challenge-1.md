# Challenge 1: Getting Started with GitHub Copilot

### Estimated Time: ? minutes

## Overview

Getting started with GitHub Copilot involves a seamless setup process within Visual Studio Code (VS Code). To begin, install the GitHub Copilot extension from the VS Code marketplace and log in with your GitHub account for an enhanced coding experience. Familiarize yourself with the GitHub Codespaces integration, which facilitates collaborative coding in a cloud-based environment. As you delve into the features, GitHub Copilot showcases its prowess in code autocompletion, providing context-aware suggestions and streamlining the development process. Moving on to code generation, experiment with Copilot's capabilities by creating simple Python and JavaScript scripts. For instance, build a basic calculator or develop an application that retrieves weather data from APIs, witnessing Copilot's ability to generate code snippets based on your context. Additionally, explore Copilot Chat to interactively communicate and refine code generation through feedback. Lastly, embrace Copilot's support for code refactoring and debugging, empowering developers to enhance code quality and identify and fix issues efficiently. In essence, GitHub Copilot serves as a powerful coding companion, accelerating development workflows and fostering code quality and collaboration.

## Introduction

**GitHub Copilot** is a groundbreaking AI-powered coding companion seamlessly integrated into Visual Studio Code, designed to enhance your coding experience. By leveraging machine learning, Copilot assists developers in crafting code by intelligently suggesting completions and generating contextually relevant code snippets.

Imagine navigating a complex coding project and encountering puzzles that demand meticulous attention to detail. GitHub Copilot steps in as your coding ally, offering insightful suggestions and autocompletions tailored to the coding context. This not only boosts coding efficiency but also serves as a valuable learning tool, providing a deeper understanding of coding structures and patterns.

But that's not all—explore the integration of GitHub Copilot with GitHub Codespaces, a feature that extends the collaborative potential of your coding environment. This integration opens up new avenues for collaborative coding, enabling teams to work seamlessly on projects regardless of geographical boundaries.

In this challenge series, you'll dive into GitHub Copilot's capabilities, starting with the setup and exploration of its features. From collaborative coding with GitHub Codespaces to experimenting with Copilot's suggestions and creating code for various tasks, you'll embark on a journey to harness the full potential of this revolutionary coding assistant.

## Prerequisites

Make sure you have the following from the CloudLabs provided integrated environment:

> **Note**: Pre-requisites are already set-up in the CloudLabs provided environment. If you're using your personal computer or laptop, please make sure that all necessary prerequisites are installed to complete this Hackathon.

- [Visual Studio Code](https://code.visualstudio.com/)
- [GitHub account](https://github.com/)
- [GitHub Copilot extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) installed in VS Code.

## Challenge Objectives:

1. **Setup GitHub Copilot in VS Code:**
   - Install the GitHub Copilot extension from the VS Code Marketplace.
   - Configure the extension settings to suit your preferences.

2. **Login with GitHub Account:**
   - Login to GitHub within Visual Studio Code using the provided GitHub credentials.

3. **Using GitHub Codespaces with Copilot:**
   - Explore the integration of GitHub Codespaces with GitHub Copilot.
   - Understand how Copilot can be utilized in a collaborative coding environment.

4. **Explore GitHub Copilot Features:**
   - Experiment with Copilot in various coding scenarios.
   - Use Copilot's suggestions to speed up your code writing process.

5. **Code Generation with Copilot and Copilot Chat:**
   - Create a Python/JS based code to build a calculator.
      - Utilize GitHub Copilot to generate Python or JavaScript code that creates a basic calculator.
      - Experiment with different mathematical operations and user interactions.
   - Create a Python/JS based app to get weather data from weather APIs.
      - Leverage Copilot to generate Python code that interacts with weather APIs to retrieve weather data.
      - Explore the integration of JSON for handling and parsing weather data.

6. **Code Refactoring & Debugging:**
   - Refactor given code snippets using Copilot, understanding the process of code improvement.

      ```
      #A poorly written example of a program in Python. It prompts the user for the number of elements to sum, takes those integers as input, and handles some basic error cases
      
      MAX = 100

      def calculate_sum(arr):
         result = 0
         for num in arr:
            result += num
         return result

      def main():
         try:
            n = int(input("Enter the number of elements (1-100): "))
            if not 1 <= n <= MAX:
                  print("Invalid input. Please provide a digit ranging from 1 to 100.")
                  exit(1)

            arr = []

            print(f"Enter {n} integers:")
            for _ in range(n):
                  try:
                     arr.append(int(input()))
                  except ValueError:
                     print("Invalid input. Please enter valid integers.")
                     exit(1)

            total = calculate_sum(arr)

            print("Sum of the numbers:", total)

         except KeyboardInterrupt:
            print("\nProgram terminated by user.")
            exit(1)

      if __name__ == "__main__":
         main()
      ```
   - Debug code effectively with Copilot's assistance, addressing and fixing identified issues.

      ```
      # Intentionally flawed Python program

      # importing modules
      import itertools, random

      # make a deck of cards
      deck = list(itertools.product(range(1,14),['Spade','Heart','Diamond','Club'])

      # shuffle the cards
      random.shuffle(deck)

      # draw five cards
      print("You got:")
      for i in range(5)
         print(deck[i][0], "of", deck[i][1]

      ```

## Success Criteria:

- GitHub Copilot is successfully installed and configured in Visual Studio Code.
- You have logged in to your GitHub account within VS Code.
- You've explored GitHub Codespaces integration and understand its collaboration features.
- Successfully tried out Copilot in coding scenarios, experiencing its code generation capabilities.
- Created Python/JS code for a calculator and an app to get weather data using Copilot.
- Successfully refactor a chosen piece of code, improving its readability and overall quality.
- Successfully fix a piece of code with intentional errors using Copilot's suggestions.


## Additional Resources:

- [GitHub Copilot Documentation](https://github.com/github/copilot-docs)
- [GitHub Codespaces Documentation](https://docs.github.com/en/codespaces)

### Conclusion

In this challenge, you successfully set up GitHub Copilot in Visual Studio Code, configured extension settings, and logged in with your GitHub account. You explored the integration of GitHub Codespaces with Copilot, experiencing its collaborative coding potential. Throughout the challenge, you experimented with Copilot's features, speeding up your coding process, and completed tasks such as creating Python/JS code for a calculator and an app to fetch weather data. Additionally, you refined your coding skills by refactoring code snippets and debugging with Copilot's assistance. These accomplishments provide a solid foundation for the upcoming challenges, where you'll further explore the capabilities of GitHub Copilot.
