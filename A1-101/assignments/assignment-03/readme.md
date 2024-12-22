# **Python Assignment 03**

## **Overview**

In this assignment, you’ll practice the following Python fundamentals:

1. **Variables and basic data types (strings, integers, floats).**
2. **Getting user input and type casting.**
3. **String methods** (e.g., `upper()`, `lower()`, `strip()`, `replace()`, etc.).
4. **Basic arithmetic with numbers.**
5. **List creation, indexing, and methods** (`append()`, `remove()`, slicing, etc.).

## **The assignment is broken into several parts. Complete the core tasks first (Parts 1–3), and then try the extra challenges (Part 4) if you want to go deeper.**

## **Part 1: Working with Variables, Input, and Strings**

1. **Prompt for user input**

   - Ask the user to enter their full name and store it in a variable named `full_name`.
   - Print a greeting message, for example:

   ```python
   Hello, <full_name>! Welcome to the Python assignment.
   ```

2. **String methods**

   - Print the user’s name in **all uppercase** letters.
   - Print the user’s name in **all lowercase** letters.
   - Print the **length** of the user’s name (number of characters).
   - Replace all the **spaces** in the user’s name with **hyphens** (`-`), and print the result.
   - **Bonus**: Trim any leading or trailing spaces (if any) from the user’s name using `strip()`.

3. **Type casting and numeric operations**

   - Ask the user to enter their **birth year** (as input). Convert that input to an integer.
   - Calculate the user’s approximate age by subtracting the birth year from the **current year**. Print the result in a sentence.
   - Example output:

   ```python
   You are approximately 25 years old.
   ```

---

## **Part 2: Lists and Indexing**

1. **Create a list from user input**

   - Prompt the user to enter three of their favorite fruits (e.g., `"apple,banana,orange"`) in one line, separated by **commas**.
   - Split the string by commas to create a list called `fruit_list`.
   - Print the list to verify that it’s correct.

2. **List indexing and slicing**

   - Print the **first** fruit in the list.
   - Print the **last** fruit in the list.
   - Print the **second** fruit in the list using indexing (i.e., `fruit_list[1]`).
   - Print the **slice** of the list containing the first two fruits.

3. **List methods**
   - **Append** a new fruit to the list using `append()`. Print the updated list.
   - **Remove** one fruit from the list using `remove()` (or `pop()`). Print the updated list again.
   - Print the **length** of the list using `len()`.

---

## **Part 3 (Optional Challenge): Combining Concepts**

1. **String & List Interaction**

   - Create a new list from the letters of your `full_name` (excluding spaces).

     **Hint**:

     ```python
     letters_list = list(full_name.replace(" ", ""))
     ```

   - Print the **first 3 letters** and the **last 3 letters** of `letters_list`.

2. **Manipulate and Reconstruct**

   - Convert the **first 3 letters** of `letters_list` to uppercase, and the **rest** to lowercase.
   - Reconstruct the name from `letters_list` back into a string using `"".join(...)` and print it out.

3. **Simple Arithmetic on a List of Numbers**
   - Prompt the user to enter **5 numbers** (e.g., `"10 20 30 40 50"`) in one line, separated by spaces.
   - Convert each input into an integer and store all in a list called `numbers_list`.
   - Print the **sum** of the numbers, and the **average** (sum / length of the list).

---

## **Part 4: Additional Questions & Mini-Challenges**

If you’d like to push your understanding further, try these extra questions:

1. **Fruit List Enhancements**

   - After creating your `fruit_list`, ask the user if they want to **sort** the list alphabetically.
     - If “yes,” then sort the list and print it.
     - If “no,” do nothing.
   - Print the **longest** fruit name and the **shortest** fruit name from the list (by string length).

2. **Searching in the Fruit List**

   - Prompt the user for the name of a fruit.
   - Check if that fruit is **in** the list.
     - If it is, print “Fruit found at index X.”
     - If not, print “Fruit not found.”

3. **Name Palindrome Check (String Manipulation)**

   - Check if the user’s `full_name`, **ignoring spaces**, is a palindrome.
   - A palindrome reads the same forwards and backwards (e.g., “racecar”).
   - Print a message indicating whether it is or isn’t a palindrome.
   - _Hint_: Convert the name to a version without spaces and in one consistent case (e.g., all lowercase) before you check.

4. **Enhanced Number Operations**

   - After the user enters 5 numbers, also print:
     - The **minimum** and **maximum** values in the list.
     - The **product** of all the numbers (e.g., `num1 * num2 * ... * num5`).

5. **Reflection Questions**
   - **RQ1**: Why do we need to convert user input (strings) to integers before doing numeric operations?
   - **RQ2**: Could there be any issues if the user enters a non-numeric value where a number is expected? How might you handle that?
   - **RQ3**: Why might slicing and indexing be helpful when working with strings or lists?
   - **RQ4**: What are the advantages or disadvantages of storing user data in multiple variables vs. storing them in a single list?

---

## **Example Output (Walkthrough)**

```text
(Part-1 Output)

Enter your full name:  John Doe
Hello, John Doe! Welcome to the Python assignment.
Your name in uppercase: JOHN DOE
Your name in lowercase: john doe
Length of your name: 8
Name with hyphens: John-Doe
Current year is 2024, so you are approximately 24 years old.

(Part-2 Output)

Enter three of your favorite fruits (comma-separated): apple, banana, mango
Your list of fruits: ['apple', ' banana', ' mango']
First fruit: apple
Last fruit:  mango
Second fruit:  banana
First two fruits: ['apple', ' banana']
Adding a new fruit...
Updated list: ['apple', ' banana', ' mango', 'strawberry']
Removing one fruit...
Updated list: ['apple', ' banana', 'strawberry']
Length of the list is now 3

(Part-3 Output)

Creating a letters list from your full name...
First 3 letters: ['J', 'o', 'h']
Last 3 letters: ['D', 'o', 'e']
Reconstructing name with some modifications...
Modified name: JOHdoe
Enter 5 numbers (space-separated): 10 20 30 40 50
Sum of your numbers: 150
Average of your numbers: 30.0

(Part-4 Output)

Minimum: 10
Maximum: 50
Product: 12000000

Is your name a palindrome? (Ignoring spaces): No
Longest fruit in your list: strawberry
Shortest fruit in your list: apple
```

_(Note: The above output is just an illustration. Actual outputs may vary.)_

---

## **Submission Guidelines:**

1. **Submission Options:**
   - **Option 1**: Create a Google Colab file (`Your PIAIC_RollNumber.ipynb`) and ensure the permissions are set to "Anyone with the link can view." Submit the link in Google Classroom.
   - **Reflection**: Include **brief answers** to the reflection questions as comments in your code (e.g., `# RQ1: [Your answer]`).
   - **Option 2**: Add comments in your code to explain what each part does.
2. **Submission Method:** Submit your completed work through the Google Classroom assignment submission portal.

---

## **Deadline:**

- **Time:** 11:59 PM on 28/12/2024.
- **Note:** The deadline will **not be extended** under any circumstances. Please plan accordingly.

---

Good luck, and have fun coding! 🎉 You're off to a great start, future Python pro! 🚀
