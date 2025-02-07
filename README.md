Maze-Pathfinding-with-BFS-DFS-in-Java

## Overview
This project implements a graphical maze solver using Java Swing. It generates a random maze and allows the user to solve it using either the Breadth-First Search (BFS) or Depth-First Search (DFS) algorithms. The graphical representation of the maze is displayed in a JFrame, and buttons are provided to initiate the search algorithms.

## Features
- Generates a random grid-based maze.
- Implements BFS and DFS for pathfinding.
- Visualizes the search process and highlights the shortest path found (if any).
- Interactive GUI using Java Swing.

## Installation
1. Ensure you have Java installed (JDK 8 or later).
2. Clone or download this repository.
3. Compile the Java files using:
   ```sh
   javac maze.java
   ```
4. Run the program using:
   ```sh
   java maze
   ```

## Usage
- The maze is displayed as a grid, where:
  - White cells represent open paths.
  - Black cells represent obstacles.
  - The start point is the top-left corner.
  - The destination is the bottom-right corner.
- Click the **BFS** button to solve the maze using Breadth-First Search.
- Click the **DFS** button to solve the maze using Depth-First Search.
- The shortest path (if found) is highlighted in **blue**.

## How It Works
### Grid Generation
- The maze is represented as a 67x110 grid.
- Each cell is randomly set to either an obstacle or an open path.
- The start (0,0) and end (66,109) points are always open.

### BFS Algorithm
- Uses a queue to explore the maze in a breadth-first manner.
- Ensures the shortest path is found (if one exists).
- The visited nodes are tracked to prevent revisiting.

### DFS Algorithm
- Uses a stack to explore the maze in a depth-first manner.
- Introduces randomness in the order of exploration to create variety.
- May not always find the shortest path due to its backtracking nature.

## Code Structure
- **Grid.java**: Handles drawing the maze and the path visualization.
- **maze.java**:
  - Initializes the maze and GUI.
  - Implements BFS and DFS search algorithms.
  - Handles user interaction via buttons.

