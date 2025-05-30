# Metro Simulation Project
The aim of this project is to calculate the route with the least transfers and the fastest time between metro lines and stations using A* and BFS.

First of all, we can examine the node-edge visualization showing the metro lines, transfers and the kilometers between two stations with the network library.

![Ekran Görüntüsü](https://github.com/ecessuvural/MetroSimulation/raw/main/images/Ekran%20g%C3%B6r%C3%BCnt%C3%BCs%C3%BC%202025-03-23%20172040.png)



## BFS Algorithm
An technique called BFS (Breadth-First Search) is used to determine the shortest path in tree or graph topologies.  It begins at the beginning and proceeds in order to the nodes in each level.

**BFS Steps:** 

**Starting Node:** The initial location is chosen.

**Queue Structure:** The queue gains nodes.

**Finding Neighbours:** The next node's neighbours are found and added to the queue.

**Tracking Visited Nodes:** Nodes that have been visited are indicated.

As a result, BFS visits each node based on its level and determines the shortest path.

## A* Algorithm
The A* (A-star) algorithm is a search algorithm that finds the shortest path through a graph.

 __Steps for the A* Algorithm:__
 
 **Selecting the Starting Node:** The starting point is selected, and the f value is computed.

 **Using Open and Closed Lists:** The open list contains unknown nodes, whereas the closed list has processed nodes.

 **Calculating F Value:** F value is determined as f(n) = g(n) + h(n).

 **Selecting the Node With the Smallest F Value:** The node with the smallest F value in the open list is chosen.

 **Processing Neighbors:** Neighbour processing involves calculating and adding f, g, and h values from neighbouring nodes to the open list.

 **Reaching the Destination:** When the destination is reached, the algorithm returns the shortest route.

## Why were these algorithms used?
Because the BFS and A* algorithms are both efficient for shortest path and effective search, we used both.

 BFS ensures the shortest path by equally exploring each neighbour at each step.


 A*, on the other hand, concentrates on the goal, achieves quicker outcomes, and offers the quickest route to the goal.

 For big structures like metro networks, both techniques perform well.

 ## Libraries Used and Their Purposes
 
**defaultdict:** If a given key is not present in this data structure, a default value is returned (such as a list or a number).  This helps to prevent errors.

**heapq:** Used for fast finding a small value or sorting the smallest items.

**dict:** A data structure made up of key-value pairs.  Both keys and values must be of specific types.

**list:** A well-structured and adaptable collection.

**set:** A collection of distinct pieces that are not in order.  You can't add the same element more than once.

**tuple:** An immutable, ordered, fixed-length collection.  It may include a variety of aspects.

**optional:** Shows that a variable can have the value None or be of the type that is defined.

**matplotlib:** It is an extremely potent Python graphing and visualisation library.  Several graph types, including pie charts, bar graphs, and line graphs, can be made with the pyplot package.

**network:** A Python library for networks (graphs) and network theory.  Graphs with nodes and edges are modelled and analysed using it.

## Examples and Results



![Scenario4](https://github.com/ecessuvural/MetroSimulation/blob/main/images/Ekran%20g%C3%B6r%C3%BCnt%C3%BCs%C3%BC%202025-03-23%20164917.png?raw=true)

![Ekran Görüntüsü](https://github.com/ecessuvural/MetroSimulation/raw/main/images/Ekran%20g%C3%B6r%C3%BCnt%C3%BCs%C3%BC%202025-03-23%20171948.png)

As can be seen, the duration of the fastest route with the fewest transfers from Keçiören to Demetevler has been calculated.

BFS was used for the fewest transfers and A* was used for the fastest route and duration calculation. The contents of the algorithm and other test examples can be accessed from the project file.

We can also examine the graph comparing the fastest route times for 4 different scenarios in the project file. This method can make comparisons easier when there are multiple scenarios.

![Ekran Görüntüsü](https://github.com/ecessuvural/MetroSimulation/raw/main/images/Ekran%20g%C3%B6r%C3%BCnt%C3%BCs%C3%BC%202025-03-23%20174021.png)

## Project Development Ideas

**UI and Notification:** If the project is to be implemented as an application, the UI design can be developed and various notifications can be sent to the user according to the metro line the user wants.

**Artificial Intelligence Support:** In this way, the user can ask questions to the artificial intelligence about the routes they will take and receive support such as directions, location suggestions specific to the route they will take, etc.

**Statistics and Data Analysis:** By examining the busiest lines and hours, density information can be provided to the user.

**Suggestions:** Route suggestions can be made according to the user's wishes. These may include information about the malfunction status of the metro or how many minutes remain until it reaches the station.






 

