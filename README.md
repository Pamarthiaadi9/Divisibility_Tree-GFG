# Divisibility_Tree-GFG
Given a tree with n nodes numbered from 1 to n and n - 1 edges connecting them. The tree is rooted at node 1. Your task is to remove a maximum number of edges from the given tree such that the tree converts into a disjoint union tree and the nodes of connected components left are divisible by 2. If n is odd, then it is allowed to keep exactly one component with an odd number of nodes. 

Example 1:
Input: 
n = 10
edges = {{2,1},{3,1},{4,3},{5,2},{6,1},{7,2},{8,6},{9,8},{10,8}}
Output:
2
Explanation:
Take two integers at a time i.e. 2 is connected with 1, 3 is connected with 1,4 is 
connected with 3, 5 is connected with 2 and so on. Fig will understand you better.
Original tree:
![image](https://github.com/Pamarthiaadi9/Divisibility_Tree-GFG/assets/105631285/ef626f15-810f-4856-8e9e-c0cee82bc524)
After removing edge 1-3 and 1-6. So ans is 2 because all nodes are even.
![image](https://github.com/Pamarthiaadi9/Divisibility_Tree-GFG/assets/105631285/cb163afe-453a-4315-b4b6-52cc720adb59)


Example 2:
Input: 
n = 4
edges = {{2,1},{4,2},{1,3}}
Output:
1
Explanation:
Removing the edge 2-1 will convert the tree into disjoint union tree with nodes of connected component left is divisible by 2. 
Your Task:
You don't need to read or print anyhting. Your task is to complete the function minimumEdgeRemove() which takes n and edges as input parameter and returns the minimum number of edges which is removed to make the tree disjoint union tree such that the tree converts into disjoint union tree so that nodes of connected component left is divisible by 2.

Expected Time Compelxity: O(n)
Expected Space Comeplxity: O(1)

Constraints:
1 <= n <= 105
edges.length == n - 1
1 <= edges[i][0], edges[i][1] <= n
