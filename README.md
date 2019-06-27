# Student Names:
* Abdullah Galal - 33821
* Sara Abdelkhalek - 33789
* Shrouk Ragheb - 33799


# Project-Social-Media-Analysis
* The project aims at applying algorithms based on graph theory to compute the centrality property for each node in the graph.
* Centrality has many definitions. Each definition gives scores to nodes in different ways.

****we are asked to implement three centrality metrics on undirected connected graphs:****
1. ***Degree Centrality:***
   - Degree centrality measures the number of incoming and outgoing relationships from a node.
     - #### Steps  :
       - take inputs from user n(nodes),m(edges)
       - make a dynamic array with size n , initial = 0
       - take inputs a(V1),b(V2),c(E between V1 & V2)
       - increase arr[V1]& arr[V2] by 1 , then repeat 
       - cout each element in arr with its degree >> example : g(V1) = 3 "degree centrality of V1" 
 
2. ***Closeness centrality:***
   - Closeness centrality is a way of detecting nodes that are able to spread information very efficiently through a graph.
  The closeness centrality of a node measures its average farness (inverse distance) to all other nodes.
  Nodes with a high closeness score have the shortest distances to all other nodes.
     - #### Steps :
       - for each node ,find the shortest distance to all other nodes 
       - calculate the Sum of all distances >> *sum += distance[j]*
       - then calculate >> Closeness = (n - 1) /sum    :n(nodes)

3. ***Betweenness Centrality:*** 
   - Betweenness centrality measures the number of times a node lies on the shortest path between other nodes.
     - #### Steps :
       - for each node ,find the shortest distance to all other nodes  >> paths 
       - then, calculate the number of times this node lies on the shortest path between other nodes >> count 
       - Betweenness centrality of node = (count / paths) 


## Graph Visualization
  - After calculating centrality using previous methods,We started to visualize graphs.
We wanted to show the degree of centrality of each node in the graph.
Nodes with larger degree of centrality are represented with larger size.
    - #### Steps :
      - Learn how to use NetworkX (is a Paython package).
      - Install networkX.
      - Send nodes , edges and degree of centrality of each node to text file from C++ program.
      - Receive data from text file.
      - Draw the graph.
