## Description

<div><p><span class="tex-font-style-it">This problem consists of two subproblems: for solving subproblem E1 you will receive 11 points, and for solving subproblem E2 you will receive 13 points.</span></p><p>A tree is an undirected connected graph containing no cycles. The distance between two nodes in an unweighted tree is the minimum number of edges that have to be traversed to get from one node to another.</p><p>You are given 3 trees that have to be united into a single tree by adding two edges between these trees. Each of these edges can connect any pair of nodes from two trees. After the trees are connected, the distances between all unordered pairs of nodes in the united tree should be computed. What is the maximum possible value of the sum of these distances?</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> — the number of vertices in the first, second, and third trees, respectively. The following <span class="tex-span"><i>n</i><sub class="lower-index">1</sub> - 1</span> lines describe the first tree. Each of these lines describes an edge in the first tree and contains a pair of integers separated by a single space — the numeric labels of vertices connected by the edge. The following <span class="tex-span"><i>n</i><sub class="lower-index">2</sub> - 1</span> lines describe the second tree in the same fashion, and the <span class="tex-span"><i>n</i><sub class="lower-index">3</sub> - 1</span> lines after that similarly describe the third tree. The vertices in each tree are numbered with consecutive integers starting with <span class="tex-span">1</span>.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem E1 (11 points), the number of vertices in each tree will be between <span class="tex-span">1</span> and <span class="tex-span">1000</span>, inclusive. </li><li> In subproblem E2 (13 points), the number of vertices in each tree will be between <span class="tex-span">1</span> and <span class="tex-span">100000</span>, inclusive. </li></ul></div><div class="output-specification"><p>Print a single integer number — the maximum possible sum of distances between all pairs of nodes in the united tree.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> — the number of vertices in the first, second, and third trees, respectively. The following <span class="tex-span"><i>n</i><sub class="lower-index">1</sub> - 1</span> lines describe the first tree. Each of these lines describes an edge in the first tree and contains a pair of integers separated by a single space — the numeric labels of vertices connected by the edge. The following <span class="tex-span"><i>n</i><sub class="lower-index">2</sub> - 1</span> lines describe the second tree in the same fashion, and the <span class="tex-span"><i>n</i><sub class="lower-index">3</sub> - 1</span> lines after that similarly describe the third tree. The vertices in each tree are numbered with consecutive integers starting with <span class="tex-span">1</span>.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem E1 (11 points), the number of vertices in each tree will be between <span class="tex-span">1</span> and <span class="tex-span">1000</span>, inclusive. </li><li> In subproblem E2 (13 points), the number of vertices in each tree will be between <span class="tex-span">1</span> and <span class="tex-span">100000</span>, inclusive. </li></ul>

## Output

<p>Print a single integer number — the maximum possible sum of distances between all pairs of nodes in the united tree.</p>





```input1
2 2 3
1 2
1 2
1 2
2 3

```




```input2
5 1 4
1 2
2 5
3 4
4 2
1 2
1 3
1 4

```




```output1
56

```




```output2
151

```



## Note

<p>Consider the first test case. There are two trees composed of two nodes, and one tree with three nodes. The maximum possible answer is obtained if the trees are connected in a single chain of 7 vertices.</p><p>In the second test case, a possible choice of new edges to obtain the maximum answer is the following: </p><ul> <li> Connect node 3 from the first tree to node 1 from the second tree; </li><li> Connect node 2 from the third tree to node 1 from the second tree. </li></ul>
