# Tree Garden Simulation

This C program simulates a tree garden, allowing users to input information about trees, storing the data in a binary file, and displaying relevant statistics.

## Table of Contents
- [Overview](#overview)
- [Usage](#usage)
- [File Structure](#file-structure)
- [How It Works](#how-it-works)
- [Sample Output](#sample-output)
- [Contributing](#contributing)
- [License](#license)

## Overview

The program utilizes a structure named `Tree` to represent individual trees with attributes such as age, water needed, and position (x, y) in the garden. Users input information for a specified number of trees, and the program saves the data to a binary file named `data.txt`. The program then reads the data from the file, displays tree information, and populates a virtual garden array. Finally, it calculates and displays the average age of the trees.

## Usage

1. **Compile the Code:**
   ```bash
   gcc tree_garden.c -o tree_garden
   ```

2. **Run the Executable:**
   ```bash
   ./tree_garden
   ```

3. **Follow On-screen Prompts:**
   - Enter the number of trees.
   - Input age, water, x, and y for each tree.

4. **Review Output:**
   - Tree information, garden array, and average age are displayed.

## File Structure

- **tree_garden.c**: The main C program file.
- **data.txt**: Binary file to store tree data.

## How It Works

1. **User Input:**
   - The program prompts the user to input the number of trees and details for each tree.
   - Tree data is stored in the `data.txt` binary file.

2. **Data Reading and Display:**
   - The program reads tree data from `data.txt` and displays individual tree information.

3. **Garden Population:**
   - The program initializes a virtual garden array.
   - Tree ages are populated in the garden array based on their positions.

4. **Output:**
   - The program displays the garden array and calculates the average age of the trees.

5. **Memory Management:**
   - Dynamically allocated memory for the array of `Tree` structures is freed.

## Sample Output

```plaintext
Please enter the number of trees: 3
Enter age, water, x, y for tree N1:
10 20 5 10
Enter age, water, x, y for tree N2:
15 25 8 15
Enter age, water, x, y for tree N3:
12 18 12 20

Tree at position (5, 10): 10-year-old, Water Needed: 20 liters
Tree at position (8, 15): 15-year-old, Water Needed: 25 liters
Tree at position (12, 20): 12-year-old, Water Needed: 18 liters

Age: 10, Water Needed: 20, Position: 5 10
Age: 15, Water Needed: 25, Position: 8 15
Age: 12, Water Needed: 18, Position: 12 20

  0  0  0  0  0  0  0  0  0  0 10  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0
  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0
  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0
  0  0  0  0  0  0  0  
