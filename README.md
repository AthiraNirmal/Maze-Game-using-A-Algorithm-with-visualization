# Maze-Game-using-A-Algorithm-with-visualization
                                                    I. PROBLEM
To develop a game board which aims to find path from starting point to destination on a n*n box. There will be a user starting from first block who has to reach some designated block. On the way some in some cells there will be opponents who has some weights. Whenever user comes across one opponent, he will lose some points (representing low health points). If the point of user drops to zero, the game is over. The algorithm will find the path with maximum points. The algorithm used is A* algorithm along with the visualization.

                                                  II. A* ALGORITHM
A* is a very efficient algorithm and initially, the prime objective of the Algorithm was graph traversal problem to find the shortest path between two points. For the given problem statement, we implemented this approach to find the path which will have largest weights. A* actually extends the Dijkstra's algorithm along with some characteristics of breadth-first search (BFS). The main backbone of the algorithm is the heuristic function h, f and g. The heuristic function calculates the estimated total points from current node to end node, whereas the g function calculates the distance from start node to current node. The function f is the sum of both h and g. The next node to traverse is chosen according to the f value.

                                        III. SOFTWARE DESIGN AND IMPLEMENTATION
A. SoftwareDesign

First we have to initialize the open_list and closed_list and add the starting cell to the open_list. For each node in open_list, we check for any children nodes possible. We traverse through the matrix until there are no more child nodes or until we reach the destination node. The next node is selected based on the calculated f value of each child node. The node with greatest f value will be taken as the next node. The h value is dependent on the weight each cell possess. The function is called recursively till the open_list is empty.

B. Implementation and Tools Used
Here, A* is implemented in Python as per the algorithm. For the visualization purpose, we can use the turtle package of Python.


<img width="817" alt="Screen Shot 2022-07-15 at 6 41 19 PM" src="https://user-images.githubusercontent.com/63495996/179320932-7d3c723c-7f67-4e04-b385-4f8e357c749a.png">


<img width="1023" alt="Screen Shot 2022-07-15 at 6 42 15 PM" src="https://user-images.githubusercontent.com/63495996/179321031-cfc8f7c1-bc84-4149-ac1e-120836c4dccf.png">
