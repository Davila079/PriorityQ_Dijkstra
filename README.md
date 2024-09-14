# Implementation of Dijkstra’s Algorithm for Finding the Shortest Path in a Graph

In this implementation, we utilize Dijkstra’s algorithm to find the shortest path between two nodes in a graph. Below, I’ll describe the key steps involved in this process:

## Initialization:
   - We set the distance from the source node to itself as 0, and all other distances as infinity (represented by a large value, such as INT_MAX).
   - We create an empty set called “S” to store visited nodes.
   - Initialize a priority queue (or a queue called “Q”) with all nodes in the graph.
## Main Loop:
   - While the priority queue is not empty:
   - Select the node “u” from the queue with the minimum distance.
   - Add “u” to the set “S.”
   - Update distances to neighboring nodes of “u” if a shorter path is found.
## Node Exploration:
   - During the algorithm’s execution, we traverse nodes and enqueue their adjacent nodes into the priority queue.
   - We accumulate distances of visited nodes and dequeue them.
   - We maintain an array called “parent” to track the path from the source node to the current node.
## Distance Updates:
   - In the main loop, we find the unvisited node with the minimum distance in the priority queue.
   - Explore adjacent nodes of the current node.
   - If a shorter path to an adjacent node is discovered, update its distance, parent node, and enqueue it.
## Printing the Shortest Path:
   - At the end of the algorithm, we print the names of nodes that form the shortest path, along with the total distance traveled.
## User Input:
   - We’ve included a function that allows the user to input the names of the source and destination states using text.
   - If an incorrect or unavailable state is entered, a warning is displayed, and the user is prompted to re-enter the information.

This implementation uses this node map as a reference, but in the files edges.txt and vertices.txt you can add or edit the nodes and distances.
The edges file is the following format:
- origin city
- destiny city
- distance between them

The vertices file has the node names only one time:
- firstcity
- secondcity
- thirdcity

## NodeMap used in the implementation
![Nodes](https://github.com/user-attachments/assets/30580f9b-d2da-458e-96a1-eec94dc22260)
