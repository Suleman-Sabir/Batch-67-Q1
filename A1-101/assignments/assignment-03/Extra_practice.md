# **Assignment: Python Fundamentals Through Real-World Scenarios**

In this extended version of the assignment, you will tackle **six** different real-world scenarios, each focusing on Python fundamentals:
- Variables and type casting  
- User input  
- String manipulation  
- Lists and indexing  
- List methods  
- Basic arithmetic  
- Logical thinking and problem-solving  

---

## **Scenario 1: Event Registration Desk**

### **Situation**  
You are helping organize a small social event. Guests arrive, provide their names, and you want to collect some basic information.

### **Tasks**  
1. **Collect Guest Information**  
   - Prompt the user to enter their full name.  
   - Create two variables: `first_name` and `last_name` by splitting the input on the first space (assume only one space between first and last).  
   - Print a greeting using both names. For example:  
     ```
     Welcome, <first_name> <last_name>! We’re happy to have you here.
     ```

2. **Name Formatting**  
   - Print the guest’s name in **all uppercase** letters.  
   - Print the guest’s name in **all lowercase** letters.  
   - Print the number of characters in the guest’s full name (**excluding** any leading or trailing spaces).

3. **Age Calculation**  
   - Prompt the user to enter their year of birth (as a string).  
   - Convert that string to an integer and estimate their age based on the current year (e.g., `2024 - birth_year`).  
   - Print a sentence like:  
     ```
     Thank you, <first_name>. Based on your birth year, you are approximately X years old.
     ```

4. **Reflective Question**  
   - Why do we need to convert the birth year to an integer? What would happen if we didn’t?

---

## **Scenario 2: Fruit Store Inventory**

### **Situation**  
You run a small fruit store, and you want to keep track of the fruits you have in stock, as well as manage adding/removing fruits from your inventory.

### **Tasks**  
1. **Initial Fruit List**  
   - Prompt the user to enter three fruits they currently have in stock, separated by commas (e.g., `"apples,bananas,cherries"`).  
   - Split this string into a list called `fruit_inventory`.  
   - Print the list to confirm that it’s stored correctly.

2. **Manipulating the Inventory**  
   - Print the **first** fruit in the list.  
   - Print the **last** fruit in the list.  
   - Print the **length** of `fruit_inventory`.  
   - Ask the user for one additional fruit to add. Use `append()` to add it to `fruit_inventory`. Print the updated list.  
   - Ask the user which fruit they want to remove. Use `remove()` (or `pop()`) to remove it. Print the updated list again.

3. **Stock Check**  
   - Suppose you want to check if a certain fruit is in stock. Prompt the user for a fruit name and check if it exists in `fruit_inventory`. Print a message indicating whether it’s available or not.  
   - If available, print the **index** of that fruit in the list.

4. **Reflective Question**  
   - In what scenarios would you prefer using `remove()` over `pop()`? Can you think of a situation where the index-based removal from a list is more convenient than removing by value?

---

## **Scenario 3: Quick Order Calculator**

### **Situation**  
Now you want to calculate the total cost of a customer’s order.

### **Tasks**  
1. **Order Details**  
   - Ask the user: “How many items are you purchasing?” Convert that to an integer and store it in `num_items`.  
   - Then, ask the user: “What is the price per item?” Convert that to a float and store it in `price_per_item`.  
   - Calculate the total cost as `num_items * price_per_item`.  
   - Print the total cost in a sentence like:  
     ```
     Your total cost for <num_items> items is $<total_cost>.
     ```

2. **Discount Check**  
   - If `total_cost` is greater than \$50, print a message:  
     ```
     You qualify for a 10% discount!
     ```
   - Otherwise, print:  
     ```
     No discount available. Buy more to save!
     ```
   - *(Optional)* If you want students to apply the discount, have them recalculate the total cost after discount and print the new total.

3. **Reflective Question**  
   - Why might it be important to store `price_per_item` as a float instead of an integer? Give an example scenario where using an integer could cause a problem.

---

## **Scenario 4: Guest Name as a List (Optional Twist on Event Registration)**

### **Situation**  
Back to the event scenario: you realize you want to do some fun name-based games or name tags.

### **Tasks**  
1. **String to List Conversion**  
   - Reuse the guest’s `full_name` from Scenario 1.  
   - Remove any spaces, and convert the remaining characters into a list called `name_letters`.  
     - For example, `"John Doe"` becomes `['J', 'o', 'h', 'n', 'D', 'o', 'e']`.  
   - Print the list of letters.

2. **Modifying the Letters**  
   - Convert the **first half** of the letters to uppercase, and the **second half** to lowercase. (You can decide how to handle odd/even lengths.)  
   - Join the letters back into a single string and print the result.  
   - *Example:* For `"John Doe"` with 7 characters (`['J','o','h','n','D','o','e']`), you might do the first 3 letters uppercase, and the last 4 letters lowercase.

3. **Reflective Question**  
   - Why might splitting a string into a list of characters be useful in a real-world application or game?

---

## **Scenario 5: Grade Book Manager**

### **Situation**  
You are managing a small class of students, and you want to keep track of their names and grades.

### **Tasks**  
1. **Collect Students and Grades**  
   - Prompt the user to enter **how many students** there are (integer).  
   - Create **two** lists: `student_names` and `student_grades`.  
   - Use a **loop** to gather each student’s name and grade:  
     - Ask for the student’s name.  
     - Ask for the student’s grade (convert it to a float or int).  
     - Append each name to `student_names` and the corresponding grade to `student_grades`.

2. **Summary Statistics**  
   - Print **all students** with their corresponding grades.  
   - Calculate and print the **average grade** of the class.  
   - Identify and print the **highest** and **lowest** grade in the class.  
   - If there are multiple students with the highest or lowest grade, print **all** of their names.

3. **Reflective Question**  
   - What could be some limitations of storing student names and grades in separate lists? (Consider data alignment, sorting, etc.)

---

## **Scenario 6: Currency Converter**

### **Situation**  
You want to help customers convert their money from one currency to another.

### **Tasks**  
1. **Currency Input**  
   - Prompt the user to enter an amount of money in **US dollars** (USD).  
   - Convert the user input to a float.

2. **Conversion Logic**  
   - Ask the user for a **target currency** (e.g., EUR for Euro, GBP for British Pound, etc.).  
   - Based on the target currency, perform a **simple conversion** using a predefined conversion rate in your code.  
     - For instance, `1 USD = 0.85 EUR` (example rate).  
   - Calculate the converted amount and print a statement like:  
     ```
     $<amount_in_usd> in USD is approximately <converted_amount> in <currency>.
     ```

3. **Handling Edge Cases**  
   - If the user enters a currency code you haven’t defined, print:  
     ```
     Sorry, conversion rate for that currency is not available.
     ```

4. **Reflective Question**  
   - Why might floating-point precision be a problem here? Can you think of a scenario where small rounding errors matter a lot?

---
