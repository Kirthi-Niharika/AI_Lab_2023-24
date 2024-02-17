# Ex.No: 1  Implementation of Breadth First Search 
### DATE: 17/2/2024                                                                   
### REGISTER NUMBER : 212221040084
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:
```
graph = {
    '2':['3','4'],
    '3':['5'],
    '4':['6','7'],
    '5':['6'],
    '6':[],
    '7':['8'],
    '8':[]
}
visited=[]
queue=[]
def bfs(visited,node,graph):
    visited.append(node)
    queue.append(node)
    while queue:
        m=queue.pop(0)
        print(m, end=" ")
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)

print("BFS order is: ")
bfs(visited,'2',graph) 
```
### Output:
<img width="481" alt="Screenshot 2024-02-17 110514" src="https://github.com/Kirthi-Niharika/AI_Lab_2023-24/assets/114135005/713ba24d-1013-4a31-b10b-da273a317caa">

### Result:
Thus the breadth first search order was found sucessfully.
