#DFS vs BFS\
#Depth First Search\
DFS uses a stack to navigate a tree from the deepest points first (leaves) before points at the top levels (except for the points on the route to the leaf) and navigates graphs by prioritizing edge routes. This solution is optimum when the goal is far away from the start node (at leaf nodes or at the edges of a graph). This method makes a decision and then explores all it’s paths making it more suitable for decision trees.

#Breadth First Search\
BFS uses a queue to navigate a tree level by level from top to bottom. And navigates graphs by prioritizing the core routes. This solution is optimum when the goal is near the start node. This method considers all children/neighbors as potential goals and then traverses to them making it not suitable for decision trees.

#Similarities\
Both algorithms brute force the entire dataset looking for the goal by checking in their own ways. Thus, making them uninformed search algorithms. They have the same time complexity of O(V+E).

#Which one to use?\
IF we know some information about the goal picking the right algorithm should be easy. For example, if the goal is far away from the start, we should use DFS and if it’s close to the start, we should use BFS.
If the tree is very wide BFS might need too much memory making it impractical.
DFS is often used in simulation games like chess where we have a tree of all possible moves left. BFS would take a very long time by navigating row by row when DFS would just quickly find a leaf node that works.
BFS is often used when you need to find neighbor nodes like in GPS to find nearby locations.
