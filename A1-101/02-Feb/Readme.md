# Python Programming Q1

**Task**

You are tasked with developing a Python program to manage a student database. The user should be able to add new students or stop the input process by entering "stop." Each student's name, along with a sequentially generated ID starting from 1, should be stored in a tuple, with these tuples kept in a list. The program must check for duplicate names before adding a new student and display a message if a duplicate is found. After the input process ends, the program should first display the complete list of student tuples and then display each student's ID and name individually. Additionally, the program should show the total number of students, calculate and display the total length of all student names combined, and identify the student with the longest and shortest name using appropriate operators. Implement these operations within a function named `manage_student_database()` and ensure you call this function at the end of your code.

**Example Output:**

```yaml
Please enter the student's name (or type 'stop' to finish): Alice
Please enter the student's name (or type 'stop' to finish): Bob
Please enter the student's name (or type 'stop' to finish): Charlie
Please enter the student's name (or type 'stop' to finish): Alice
This name is already in the list.
Please enter the student's name (or type 'stop' to finish): Diana
Please enter the student's name (or type 'stop' to finish): stop

Complete List of Students (Tuples):
[(1, 'Alice'), (2, 'Bob'), (3, 'Charlie'), (4, 'Diana')]

List of Students with IDs:
ID: 1, Name: Alice
ID: 2, Name: Bob
ID: 3, Name: Charlie
ID: 4, Name: Diana

Total number of students: 4
Total length of all student names combined: 20
The student with the longest name is: Charlie
The student with the shortest name is: Bob
```

# Python Programming Q2

**Task : High Low**

We want you to gain more experience working with control flow and Booleans in Python. To do this, we are going to have you develop a game! The game is called High-Low and the way it's played goes as follows:
1. Two numbers are generated from 1 to 100 (inclusive on both ends): one for you and one for a computer, who will be your opponent. You can see your number, but not the computer's!
2. You make a guess, saying your number is either higher than or lower than the computer's number
3. If your guess matches the truth (ex. you guess your number is higher, and then your number is actually higher than the computer's), you get a point!
4. These steps make up one round of the game. The game is over after all rounds have been played.

**We've provided a sample run below.**

```bash
Welcome to the High-Low Game!
--------------------------------
Round 1
Your number is 8
Do you think your number is higher or lower than the computer's?: lower
You were right! The computer's number was 35
Your score is now 1

Round 2
Your number is 88
Do you think your number is higher or lower than the computer's?: higher
Aww, that's incorrect. The computer's number was 100
Your score is now 1

Round 3
Your number is 63
Do you think your number is higher or lower than the computer's?: higher
You were right! The computer's number was 5
Your score is now 2

Round 4
Your number is 57
Do you think your number is higher or lower than the computer's?: lower
Aww, that's incorrect. The computer's number was 57
Your score is now 2

Round 5
Your number is 22
Do you think your number is higher or lower than the computer's?: lower
Aww, that's incorrect. The computer's number was 1
Your score is now 2

Thanks for playing!
```

Here are some milestones to guide you through the problem:

**Milestone #1: Generate the random numbers**

Generate the random numbers for you and the computer. For now, print both of them out to help you test the logic in later milestones.

```bash
Welcome to the High-Low Game!
--------------------------------
The computer's number is 23
Your number is 82
```

**Milestone #2: Get the user choice**

Get user input for their choice of whether they think their number is higher or lower than the computer's number.
```bash
Welcome to the High-Low Game!
--------------------------------
The computer's number is 7
Your number is 17
Do you think your number is higher or lower than the computer's?: higher
```

**Milestone #3: Write the game logic**

Write code that maps out all the ways to win the round and prints out the results. When does the user win? How might we check for this? (Note: If you and the computer share the same number, the computer should win since your number wouldn't be higher nor lower.)

```bash
Welcome to the High-Low Game!
--------------------------------
The computer's number is 79
Your number is 3
Do you think your number is higher or lower than the computer's?: lower
You were right! The computer's number was 79
```

**Milestone #4: Play multiple rounds**

Milestones 1-3 make up a single round of the game. Now that your game logic is sound, you can remove the line printing out the computer's number. Next, write code to play multiple rounds of the game! How many rounds should they play you ask? We've provided you with the NUM_ROUNDS constant. NUM_ROUNDS is the number of rounds you should have the user play. For reference, in the first example, we had NUM_ROUNDS = 3. After each round, add a blank line to separate the rounds visually. Make sure to print out the round number as well!

```bash
Welcome to the High-Low Game!
--------------------------------
Round 1
Your number is 22
Do you think your number is higher or lower than the computer's?: lower
You were right! The computer's number was 23

Round 2
Your number is 76
Do you think your number is higher or lower than the computer's?: higher
Aww, that's incorrect. The computer's number was 81

... (more rounds are played)
```

**Milestone #5: Adding a points system**

Keep track of the player's score! You should print out the player's score after each round. After this step, you will have coded up the entire game!

**Extension #1: Safeguard user input**

Get user input for their choice of whether they think their number is higher or lower than the computer's number.

Welcome to the High-Low Game!
--------------------------------
Round 1
Your number is 1
Do you think your number is higher or lower than the computer's?: even
Please enter either higher or lower: lower
You were right! The computer's number was 6
Your score is now 1

**Extension #2: Conditional ending messages**

Add conditional messages at the end which gauge players on how they performed! For ours, we evaluated the player and gave them separate messages if:

they had a perfect game

...
Your score is now 5

Wow! You played perfectly!

they won at least half the rounds (rounded down)

...
Your score is now 2

Good job, you played really well!

they won less than half the rounds

...
Your score is now 1

Better luck next time!


# Python Programming Q3

**Task**

You are tasked with creating a Python program that serves as an interactive tool for a friend who enjoys exploring numbers. The program should begin by prompting the user to enter their name and then ask them for three of their favorite numbers. After gathering this information, the program should greet the user with a personalized message that includes their name. The three numbers provided by the user should be stored in a list. The program should then check if any of the numbers are even or odd, and store this information in a separate list of tuples, where each tuple contains the number and a string indicating whether it is "even" or "odd". Following this, the program should use a for loop to iterate over the list of numbers, and for each number, it should create a tuple containing the number and its square. These tuples should be printed in a creative and engaging format. Additionally, the program should calculate the sum of the three numbers and print the result, accompanied by an encouraging message. Finally, the program should determine if the sum is a prime number and notify the user with an appropriate message. The goal is to make the tool both enjoyable and informative, allowing the user to explore their favorite numbers in a fun and interactive way, while also introducing some interesting logical checks.

**Example Output:**
```yaml
Enter your name: Alex
Enter your first favorite number: 4
Enter your second favorite number: 6
Enter your third favorite number: 9

Hello, Alex! Let's explore your favorite numbers:
The number 4 is even.
The number 6 is even.
The number 9 is odd.
The number 4 and its square: (4, 16)
The number 6 and its square: (6, 36)
The number 9 and its square: (9, 81)

Amazing! The sum of your favorite numbers is: 19
Wow, 19 is a prime number!
```