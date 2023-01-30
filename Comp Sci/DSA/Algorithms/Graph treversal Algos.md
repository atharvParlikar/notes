There are 2 main graph traversal algorithms,
- Depth First Treversal (DFT)
- Breadth First Treversal (BFT)

### Depth First Treversal

depth first treveral as the name suggests traverses to the deepest end of a node before starting with any other neibor.

![[Pasted image 20230126112330.png]]

let's assume this graph
The traversal order of it starting from `node a` would be
iteration :=
1. a -> b -> d -> f
2. a -> c -> e

we implement this using a [[stack]]
the algo will be
1. declare the [[stack]]. 
2. push the start node to DS
3. when you push you mark it as visited
4. until the DS is not empty run a loop
5. inside loop pop the DS and save it in a new object actual
6. loop through the neighbors of actual
7. if the current neighbor n is not visited
8. then push n in DS
9. mark n as visited in the next line.


### Bredth First treversal (BFT)

breadth first treversal is similar to DFS, only difference is we explore uniformly in all directions in BFS

![[Pasted image 20230126114815.png]]

For example in the same graph as above the iterations will look like following

![[Pasted image 20230126112330.png]]
Iterations :=
1. a -> b
2. a -> c
3. a -> b -> d
4. a -> c -> e
5. a -> b -> d -> f

we implement this using a [[queue]] 
1. declare the DS [[queue]]
2. push the start node to DS
3. when you push you mark it as visited
4. until the DS is not empty run a loop
5. inside loop pop the DS(deque for queue or pop for stack) and save it in a new object actual
6. loop through the neighbors of actual
7. if the current neighbor n is not visited
8. then push n in DS
9. mark n as visited in the next line.