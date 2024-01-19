# Challenge 3: Code Refactoring & Debugging

### Estimated Time: ?

## Introduction

In this challenge, you'll dive into the world of code refactoring and debugging using GitHub Copilot. Code refactoring involves restructuring existing code to improve its readability, maintainability, and efficiency, while debugging focuses on identifying and fixing issues within the code.

GitHub Copilot, powered by advanced machine learning models, will assist you in both refactoring and debugging tasks. By leveraging Copilot's intelligent suggestions, you can enhance the quality of your code and resolve any issues efficiently.

## Challenge Objectives:

1. **Refactor a given piece of code:**
   - Choose a section of code, and refactor it to improve readability, adhere to coding standards, and enhance overall code quality.
   - Experiment with different refactoring techniques, such as simplifying complex expressions, renaming variables, and extracting methods.

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

2. **Fix a given piece of code:**
   - Identify a piece of code with intentional errors or issues.
   - Use GitHub Copilot to assist you in debugging and fixing the identified issues.
   - Explore Copilot's suggestions for error correction, and verify the effectiveness of the fixes.

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

- Successfully refactor a chosen piece of code, improving its readability and overall quality.
- Successfully fix a piece of code with intentional errors using Copilot's suggestions.

## Additional Instructions:

- Feel free to explore additional refactoring techniques beyond the provided tasks.
- Experiment with different debugging scenarios to understand Copilot's capabilities in identifying and fixing code issues.
- If you encounter any challenges or have questions, refer to the [GitHub Copilot Documentation](https://github.com/github/copilot-docs) for guidance.

## Conclusion

In this challenge, you've experienced the power of GitHub Copilot in assisting with code refactoring and debugging tasks. By leveraging Copilot's suggestions, you've not only enhanced the quality of your code but also efficiently addressed code issues. As you continue your coding journey, remember to integrate these learnings into your regular development practices for more effective and error-free coding.

Happy coding!
