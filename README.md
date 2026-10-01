# SLE-3 | BFS and DFS Graph Search System

**Architectural Design Using the Full C4 Model**

**Course:** 02AML204 – Introduction to Artificial Intelligence
**Program:** SY B.Tech. CSE (AI & ML), SEM-VI
**Student:** Shradha Kumbhar
**PRN:** 25UAM030

---

## About the Project

The **BFS and DFS Graph Search System** is a graph search system that finds a path between a starting node and a goal node.

The system supports two commonly used graph search algorithms:

**Breadth-First Search (BFS)**
**Depth-First Search (DFS)**

The user provides the graph, starting node, goal node, and selected search algorithm. The system then performs the search and provides information about the explored nodes, search result, path, and performance.

The architecture of this system is represented using the **Full C4 Model**.

---

## C4 Architecture

### Context — Level 1

The Context Diagram gives a high-level view of the complete system.

The user provides the graph and search details to the Graph Search System. The system performs BFS or DFS and returns the search result and relevant search information to the user.

**Diagram:** `diagrams/C4-Level-1-Context.png`

### Container — Level 2

The Container Diagram shows the major building blocks of the system.

| Container            | Main Responsibility                             |
| :------------------- | :---------------------------------------------- |
| Input Module         | Receives graph and search inputs from the user. |
| Search Engine        | Performs BFS or DFS.                            |
| Visited Set          | Maintains information about explored nodes.     |
| Performance Analyzer | Records search performance information.         |
| Output Module        | Presents the final search result.               |

**Diagram:** `diagrams/C4-Level-2-Container.png`

### Component — Level 3

The Component Diagram shows the internal structure of the **Search Engine**.

| Component          | Main Responsibility                                         |
| :----------------- | :---------------------------------------------------------- |
| Frontier           | Stores nodes that are waiting to be explored.               |
| Explored Set       | Maintains nodes that have already been explored.            |
| Goal Test          | Checks whether the goal node has been reached.              |
| Path Reconstructor | Reconstructs the path from the start node to the goal node. |

**Diagram:** `diagrams/C4-Level-3-Component.png`

### Code — Level 4

The Code Diagram presents the main functions involved in the search process.

| Function                | Purpose                                          |
| :---------------------- | :----------------------------------------------- |
| `bfs_search()`          | Performs Breadth-First Search.                   |
| `dfs_search()`          | Performs Depth-First Search.                     |
| `goal_test()`           | Checks whether the current node is the goal.     |
| `reconstruct_path()`    | Creates the final path using search information. |
| `measure_performance()` | Records performance information.                 |

**Diagram:** `diagrams/C4-Level-4-Code.png`

---

## System Flow

The system follows a simple flow:

**User → Input Module → Search Engine → Explored Information → Path Reconstruction → Output Module**

Each C4 level provides a different view of this same system.

The Context level focuses on the user and system interaction.
The Container level shows the major system modules.
The Component level explains the internal Search Engine.
The Code level identifies the important functions.

---

## Design Decisions

The system is divided into separate modules so that each module has a clear responsibility.

BFS and DFS are implemented as the main search operations within the Search Engine. Separate handling of explored nodes, path reconstruction, performance information, and output makes the system easier to understand and maintain.

The architecture is also connected to the BFS/DFS performance profiling work completed in SLE-2.

---

## Tools Used

| Tool         | Purpose                  |
| :----------- | :----------------------- |
| BFS and DFS  | Graph search algorithms  |
| diagrams.net | C4 architecture diagrams |
| Git          | Version control          |
| GitHub       | Repository management    |
| Markdown     | Project documentation    |

---

## AI Contribution

ChatGPT was used as an AI-assisted learning tool during the development of this project.

It helped in understanding the C4 Model, organizing the BFS/DFS system into the four architectural levels, reviewing the architecture, and improving the project documentation.

The student selected the BFS/DFS system, created and edited the diagrams, organized the repository, reviewed the architecture, and made the final design decisions.

---

## Project Structure

```text
SLE-3-BFS-DFS-C4/
│
├── diagrams/
│   ├── C4-Level-1-Context.png
│   ├── C4-Level-2-Container.png
│   ├── C4-Level-3-Component.png
│   ├── C4-Level-4-Code.png
│   └── SLE3_25UAM030_Shradha_Kumbhar.drawio
│
├── docs/
│   └── Contribution-Log.md
│
└── README.md
```

---

## Conclusion

The SLE-3 project presents the BFS and DFS Graph Search System using the complete C4 architectural model.

The four levels provide a clear view of the system, from the overall user interaction to containers, components, and important code-level functions.

The resulting architecture provides a structured and modular representation of the BFS/DFS system developed as part of the SLE-2 work.
