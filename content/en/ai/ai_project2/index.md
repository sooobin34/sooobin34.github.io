---
title: "AI Project 2 – 8 Puzzle"
subtitle: "Search Algorithms for Solving the 8-Puzzle using DFS, BFS, UCS, and A*"
summary: "Implemented DFS, BFS, UCS, and A* algorithms to solve the 8-puzzle problem and compared their performance."

type: post
date: 2025-10-10
share: false
draft: false

image:
  filename: "8puzzle.jpg"

tags:
  - Artificial Intelligence
  - Search Algorithm
  - Python
  - A*

links:
  - icon: github
    icon_pack: fab
    name: "GitHub Repository"
    url: "https://github.com/sooobin34/AI_Project2"
---

<br>

## 🧩 Project Overview
This project was developed as part of the **Artificial Intelligence course** to explore various **search algorithms** through the classic **8-puzzle problem**.  
The 8-puzzle consists of a 3×3 grid with numbered tiles, where the blank tile (0) can be moved up, down, left, or right to reach a goal configuration.  
We implemented and compared the performance of multiple search algorithms (DFS, BFS, UCS, and A*).

<br>

## 📄 Project Report
If you’d like to learn more about the project, [download the report!](/files/ai_project2_report.pdf)  
(*Note: The report is written in Korean.*)

<br>

## ⚙️ Implementation Details

### 🔹 1. Search Algorithms
- **DFS (Depth-First Search):** Stack-based search; memory-efficient but does not guarantee the optimal solution.  
- **BFS (Breadth-First Search):** Queue-based search; guarantees the shortest path but consumes more memory.  
- **UCS (Uniform Cost Search):** Considers movement cost; always finds the least-cost path.  
- **A\***: Applies a heuristic function to reach the goal efficiently with minimal cost.

<br>

### 🔹 2. Heuristic Function (for A*)
The A* search uses the **misplaced tile heuristic**,  
which counts the number of tiles that are not in their goal position.

```python
def heuristic(state, problem=None):
    misplaced = 0
    goal = [[1,2,3],[4,5,6],[7,8,0]]
    for row in range(3):
        for col in range(3):
            if state.cells[row][col] != 0 and state.cells[row][col] != goal[row][col]:
                misplaced += 1
    return misplaced
