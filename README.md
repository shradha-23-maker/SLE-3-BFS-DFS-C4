\# SLE-3: Architectural Design Using Full C4 Model



\## BFS and DFS Graph Search System



\*\*Course:\*\* 02AML204 – Introduction to Artificial Intelligence

\*\*Program:\*\* SY B.Tech. CSE (AI \& ML), SEM-VI

\*\*Student:\*\* Shradha Kumbhar

\*\*PRN:\*\* 25UAM030



\---



\## 1. Project Description



The \*\*BFS and DFS Graph Search System\*\* is a graph search system that finds a path between a starting node and a goal node.



The system supports two search algorithms:



\* \*\*Breadth-First Search (BFS)\*\*

\* \*\*Depth-First Search (DFS)\*\*



The user provides the graph, starting node, goal node, and selected search algorithm. The system processes the graph and displays the search result, visited nodes, and path information.



This SLE-3 represents the system using all four levels of the \*\*C4 Model\*\*: Context, Container, Component, and Code.



\---



\## 2. C4 Architecture



\### Level 1 – Context Diagram



The Context Diagram shows the complete system and its interaction with the user.



The user provides graph and search information to the Graph Search System. The system performs BFS or DFS and returns the search result, nodes explored, and execution information to the user.



\*\*Diagram:\*\* `diagrams/C4-Level-1-Context.png`



\---



\### Level 2 – Container Diagram



The Container Diagram shows the main building blocks of the system.



The main containers are:



1\. \*\*Input Module\*\* – Accepts the graph, start node, goal node, and selected algorithm.

2\. \*\*Search Engine\*\* – Performs BFS or DFS graph searching.

3\. \*\*Visited Set\*\* – Keeps track of nodes that have already been explored.

4\. \*\*Performance Analyzer\*\* – Measures search-related execution information.

5\. \*\*Output Module\*\* – Displays the search result and other information to the user.



\*\*Diagram:\*\* `diagrams/C4-Level-2-Container.png`



\---



\### Level 3 – Component Diagram



The Component Diagram shows the internal components of the \*\*Search Engine\*\*.



The main components are:



\* \*\*Frontier\*\* – Stores nodes that are waiting



