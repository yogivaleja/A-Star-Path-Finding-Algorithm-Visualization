# A-Star-Path-Finding-Algorithm-Visualization
A * algorithm is a searching algorithm that searches for the shortest path between the initial and the final state. It is used in various applications, such as maps. In maps the A* algorithm is used to calculate the shortest distance between the source (initial state) and the destination (final state).  
A* Search algorithm is one of the best and popular technique used in path-finding and graph traversals.


# Algorithm  
1.  Initialize the open list  
2.  Initialize the closed list  
    put the starting node on the open list (you can leave its f at zero)  
3.  while the open list is not empty  
    a) find the node with the least f on the open list, call it "q"  
    b) pop q off the open list  
    c) generate q's 8 successors and set their parents to q  
    d) for each successor  
        i) if successor is the goal, stop searchsuccessor.g = q.g + distance between successor and q successor.h = distance from goal to successor (This can be done using many ways, we will discuss three heuristics- Manhattan, Diagonal and Euclidean Heuristics)  
          successor.f = successor.g + successor.h  
        ii) if a node with the same position as successor is in the OPEN list which has a lower f than successor, skip this successor  
        iii) if a node with the same position as successor  is in the CLOSED list which has a lower f than successor, skip this successor otherwise, add  the node to the open list  
     end (for loop)  
    e) push q on the closed list  
    end (while loop)   

# Requirements  
Python 3  
Tkinter  
Pygame  

# Instructions  
Simply run main.py  

# Images
![Screenshot 2020-11-04 211021](https://user-images.githubusercontent.com/53828910/98134406-bd2aaf00-1ee4-11eb-8483-f90f04e586b9.png)


