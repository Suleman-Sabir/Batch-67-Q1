---

## **Python Practice Assignment: Adventure Game**

### **Scenario:**

You are developing a simple text-based adventure game. In this game, the player will explore different locations, collect items, and make decisions that affect their progress. Your task is to guide the player through various challenges using Python concepts like variables, loops, lists, dictionaries, and `if-else` statements.

---

### **Assignment Tasks:**

#### **Step 1: Setting Up the Game**

1. Create a list named `inventory` to keep track of the items the player collects.  
   Example:  
   ```python
   inventory = []
   ```

2. Create a dictionary named `locations` where the keys are location names and the values are short descriptions of those locations.  
   Example:  
   ```python
   locations = {
       "forest": "You are in a dark forest. You hear strange noises.",
       "cave": "You have entered a damp cave. It's very cold here.",
       "river": "You are standing by a river. The water is flowing quickly."
   }
   ```

#### **Step 2: Moving Between Locations**

3. Use a `while` loop to keep the game running until the player decides to quit.  
   - At each step, display the available locations (use the dictionary keys) and ask the player to choose where to go next.
   - If the player chooses an invalid location, display an error message and prompt them to try again.
   - When the player moves to a new location, display the description of that location (use the dictionary values).

---

#### **Step 3: Collecting Items**

4. Create another dictionary named `items` where the keys are location names and the values are items the player can find in those locations.  
   Example:  
   ```python
   items = {
       "forest": "wooden stick",
       "cave": "glowing crystal",
       "river": "shiny stone"
   }
   ```

5. When the player enters a location, check if there is an item available in that location.  
   - If there is an item, ask the player if they want to collect it.  
   - If the player chooses to collect the item, add it to their inventory (use the `append` method for lists) and display a success message.  
   - If the player chooses not to collect the item, move on without adding it to the inventory.

---

#### **Step 4: Displaying the Inventory**

6. Allow the player to type `inventory` at any time to view the items they have collected so far.  
   - Use an `if-else` block to handle this input.  
   - If the inventory is empty, display a message indicating that the inventory is empty.

---

#### **Step 5: Ending the Game**

7. Allow the player to type `quit` at any time to end the game.  
   - When the player quits, display a goodbye message along with their final inventory.

---

### **Bonus Challenge (Optional)**

8. Add a health system:  
   - Create a variable `health` and set its initial value to 100.  
   - Add random events (like an animal attack or falling into a pit) that reduce the player’s health.  
   - If the player’s health reaches 0, end the game and display a "Game Over" message.

9. Add a simple battle system:  
   - Create a list of enemies that can appear randomly in different locations.  
   - Allow the player to either fight the enemy or run away.  
   - If the player chooses to fight, reduce their health by a random amount.

---

### **Sample Output:**

```
Welcome to the Adventure Game!
Available locations: forest, cave, river
Where do you want to go? forest

You are in a dark forest. You hear strange noises.
You found a wooden stick. Do you want to collect it? (yes/no) yes
You collected the wooden stick.

Available locations: cave, river
Where do you want to go? river

You are standing by a river. The water is flowing quickly.
You found a shiny stone. Do you want to collect it? (yes/no) no

Type 'inventory' to view your items or 'quit' to end the game.
Where do you want to go? inventory

Your inventory: ['wooden stick']

Available locations: cave, river
Where do you want to go? quit

Goodbye! Your final inventory: ['wooden stick']
```

---

This assignment will help students practice:

- Using **lists** and their methods (`append`, `len`)  
- Working with **dictionaries** to map locations to descriptions and items  
- Implementing **loops** to keep the game running  
- Using **conditional statements** (`if-else`) for decision-making  
- Developing **logical thinking** by simulating a real-world scenario

---
