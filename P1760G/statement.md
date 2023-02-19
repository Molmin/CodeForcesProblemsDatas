## Description

<div><p>You are given a weighted tree with $n$ vertices. Recall that a tree is a connected graph without any cycles. A weighted tree is a tree in which each edge has a certain weight. The tree is undirected, it doesn't have a root.</p><p>Since trees bore you, you decided to challenge yourself and play a game on the given tree.</p><p>In a move, you can travel from a node to one of its neighbors (another node it has a direct edge with).</p><p>You start with a variable $x$ which is initially equal to $0$. When you pass through edge $i$, $x$ changes its value to $x ~\mathsf{XOR}~ w_i$ (where $w_i$ is the weight of the $i$-th edge). </p><p>Your task is to go from vertex $a$ to vertex $b$, but you are allowed to enter node $b$ if and only if after traveling to it, the value of $x$ will become $0$. In other words, you can travel to node $b$ only by using an edge $i$ such that $x ~\mathsf{XOR}~ w_i = 0$. Once you enter node $b$ the game ends and you win.</p><p>Additionally, you can teleport <span class="tex-font-style-bf">at most once</span> at any point in time to any vertex except vertex $b$. You can teleport from any vertex, even from $a$.</p><p>Answer with "<span class="tex-font-style-tt">YES</span>" if you can reach vertex $b$ from $a$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>Note that $\mathsf{XOR}$ represents the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains three integers $n$, $a$, and $b$ ($2 \leq n \leq 10^5$), ($1 \leq a, b \leq n; a \ne b$)&nbsp;— the number of vertices, and the starting and desired ending node respectively.</p><p>Each of the next $n-1$ lines denotes an edge of the tree. Edge $i$ is denoted by three integers $u_i$, $v_i$ and $w_i$ &nbsp;— the labels of vertices it connects ($1 \leq u_i, v_i \leq n; u_i \ne v_i; 1 \leq w_i \leq 10^9$) and the weight of the respective edge.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output "<span class="tex-font-style-tt">YES</span>" if you can reach vertex $b$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains three integers $n$, $a$, and $b$ ($2 \leq n \leq 10^5$), ($1 \leq a, b \leq n; a \ne b$)&nbsp;— the number of vertices, and the starting and desired ending node respectively.</p><p>Each of the next $n-1$ lines denotes an edge of the tree. Edge $i$ is denoted by three integers $u_i$, $v_i$ and $w_i$ &nbsp;— the labels of vertices it connects ($1 \leq u_i, v_i \leq n; u_i \ne v_i; 1 \leq w_i \leq 10^9$) and the weight of the respective edge.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output "<span class="tex-font-style-tt">YES</span>" if you can reach vertex $b$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1|2,3,4,5,6,9,10,11,12,13,14
3
5 1 4
1 3 1
2 3 2
4 3 3
3 5 1
2 1 2
1 2 2
6 2 3
1 2 1
2 3 1
3 4 1
4 5 3
5 6 5
```




```output1
YES
NO
YES
```



## Note

<p>For the first test case, we can travel from node $1$ to node $3$, $x$ changing from $0$ to $1$, then we travel from node $3$ to node $2$, $x$ becoming equal to $3$. Now, we can teleport to node $3$ and travel from node $3$ to node $4$, reaching node $b$, since $x$ became equal to $0$ in the end, so we should answer "<span class="tex-font-style-tt">YES</span>".</p><p>For the second test case, we have no moves, since we can't teleport to node $b$ and the only move we have is to travel to node $2$ which is impossible since $x$ wouldn't be equal to $0$ when reaching it, so we should answer "<span class="tex-font-style-tt">NO</span>".</p>
