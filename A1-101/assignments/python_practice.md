---

## **Assignment 1: Treasure Hunt** (Beginner)

### **Scenario:**

You are creating a simple treasure hunt game. The player starts with no items and needs to find a treasure by exploring different directions.

### **Tasks:**

1. **Create a Variable for Player's Position**  
   Use a variable `position` initialized to `0`. The treasure is at position `10`.

2. **Player Movement**  
   - Use a `while` loop to keep the game running until the player reaches the treasure.
   - Ask the player to move forward or backward by typing `"forward"` or `"backward"`.
   - Update the position accordingly (`+1` for forward, `-1` for backward).
   - If the player reaches the treasure (position `10`), print a message saying they found the treasure and end the game.
   - If the player goes below position `0`, print a warning that they can't go further backward.

3. **Bonus Challenge (Optional)**  
   Add random obstacles at certain positions. If the player encounters an obstacle, they must skip their next move.

---

## **Assignment 2: Restaurant Order System** (Easy-Medium)

### **Scenario:**

You are designing a simple restaurant order system where the user can choose items from a menu and place their order.

### **Tasks:**

1. **Create a Menu**  
   Use a dictionary `menu` where keys are item names and values are their prices. Example:  
   ```python
   menu = {
       "burger": 5,
       "pizza": 8,
       "salad": 4,
       "soda": 2
   }
   ```

2. **Taking Orders**  
   - Use a `while` loop to let the user order items until they type `"done"`.
   - Each time the user enters an item, check if it exists in the menu.
     - If it exists, add its price to the total bill.
     - If it doesn’t exist, print an error message.
   - When the user types `"done"`, display the total bill and end the program.

3. **Bonus Challenge (Optional)**  
   - Allow the user to order multiple quantities of the same item.  
   - After the order is complete, display each item ordered and its quantity along with the total bill.

---

## **Assignment 3: Secret Code Breaker** (Medium)

### **Scenario:**

You are building a game where the player has to guess a secret 4-digit code.

### **Tasks:**

1. **Generate a Secret Code**  
   Use a list of 4 random digits (between 0 and 9) as the secret code.  
   Example:  
   ```python
   secret_code = [4, 1, 3, 7]
   ```

2. **Player Guesses**  
   - Ask the player to guess the code. The player should enter 4 digits separated by spaces.
   - Compare the player's guess with the secret code:
     - If a digit is correct and in the correct position, print `"Correct digit in correct position"`.
     - If a digit is correct but in the wrong position, print `"Correct digit in wrong position"`.
     - If a digit is incorrect, print `"Incorrect digit"`.
   - Keep asking the player to guess until they get the entire code correct.

3. **Bonus Challenge (Optional)**  
   Limit the player to 10 guesses. If they don’t guess the code in 10 attempts, print a "Game Over" message.

---

## **Assignment 4: Library Management System** (Medium-Hard)

### **Scenario:**

You are building a basic library management system to manage books and allow users to borrow or return books.

### **Tasks:**

1. **Create a Book List**  
   Use a list `books` to store available books. Example:  
   ```python
   books = ["Python Basics", "Data Science 101", "AI for Beginners", "Machine Learning Advanced"]
   ```

2. **Borrowing Books**  
   - Display the list of available books.
   - Ask the user to enter the name of a book they want to borrow.
   - If the book is available, remove it from the list and print a success message.
   - If the book is not available, print a message saying the book is unavailable.

3. **Returning Books**  
   - Ask the user to enter the name of a book they want to return.
   - Add the returned book to the list and print a success message.

4. **Bonus Challenge (Optional)**  
   - Keep a history of borrowed and returned books using a dictionary `history` where keys are book names and values are lists of actions (`"borrowed"` or `"returned"`).

---

## **Assignment 5: Quiz Game** (Hard)

### **Scenario:**

You are developing a quiz game where the player has to answer multiple-choice questions.

### **Tasks:**

1. **Create a Question Bank**  
   Use a list of dictionaries where each dictionary represents a question with the following keys:  
   - `"question"`: The question text.  
   - `"options"`: A list of answer options.  
   - `"answer"`: The correct answer.  
   
   Example:  
   ```python
   questions = [
       {
           "question": "What is the capital of France?",
           "options": ["Paris", "London", "Berlin", "Madrid"],
           "answer": "Paris"
       },
       {
           "question": "Which programming language is known as the 'language of the web'?",
           "options": ["Python", "C++", "Java", "JavaScript"],
           "answer": "JavaScript"
       }
   ]
   ```

2. **Game Logic**  
   - Use a `for` loop to display each question and its options.
   - Ask the player to type their answer.
   - If the answer is correct, increase their score by 1.
   - At the end, display the player’s total score.

3. **Bonus Challenge (Optional)**  
   - Allow the player to quit the game at any point by typing `"quit"`.  
   - Display the total score and a goodbye message if they quit early.

---

## **Final Notes:**

These assignments progress from **easy** to **hard** while keeping things interesting through different real-world scenarios:

1. **Treasure Hunt** – Simple movement and decision-making (loops, variables).  
2. **Restaurant Order System** – List, dictionary, and loop-based logic.  
3. **Secret Code Breaker** – List indexing and condition handling.  
4. **Library Management** – Managing lists and user interaction.  
5. **Quiz Game** – Combining lists, dictionaries, loops, and conditionals.

---
