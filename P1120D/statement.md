## Description

<div><p>You are given a rooted tree with $n$ vertices, the root of the tree is the vertex $1$. Each vertex has some non-negative price. A leaf of the tree is a non-root vertex that has degree $1$.</p><p>Arkady and Vasily play a strange game on the tree. The game consists of three stages. On the first stage Arkady buys some non-empty set of vertices of the tree. On the second stage Vasily puts some integers into all leaves of the tree. On the third stage Arkady can perform several (possibly none) operations of the following kind: choose some vertex $v$ he bought on the first stage and some integer $x$, and then add $x$ to all integers in the leaves in the subtree of $v$. The integer $x$ can be positive, negative of zero.</p><p>A leaf $a$ is in the subtree of a vertex $b$ if and only if the simple path between $a$ and the root goes through $b$.</p><p>Arkady's task is to make all integers in the leaves equal to zero. What is the minimum total cost $s$ he has to pay on the first stage to guarantee his own win independently of the integers Vasily puts on the second stage? Also, we ask you to find all such vertices that there is an optimal (i.e. with cost $s$) set of vertices containing this one such that Arkady can guarantee his own win buying this set on the first stage.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 200\,000$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($0 \le c_i \le 10^9$), where $c_i$ is the price of the $i$-th vertex.</p><p>Each of the next $n - 1$ lines contains two integers $a$ and $b$ ($1 \le a, b \le n$), denoting an edge of the tree.</p></div><div class="output-specification"><p>In the first line print two integers: the minimum possible cost $s$ Arkady has to pay to guarantee his own win, and the number of vertices $k$ that belong to at least one optimal set.</p><p>In the second line print $k$ distinct integers <span class="tex-font-style-bf">in increasing order</span> the indices of the vertices that belong to at least one optimal set.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 200\,000$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($0 \le c_i \le 10^9$), where $c_i$ is the price of the $i$-th vertex.</p><p>Each of the next $n - 1$ lines contains two integers $a$ and $b$ ($1 \le a, b \le n$), denoting an edge of the tree.</p>

## Output

<p>In the first line print two integers: the minimum possible cost $s$ Arkady has to pay to guarantee his own win, and the number of vertices $k$ that belong to at least one optimal set.</p><p>In the second line print $k$ distinct integers <span class="tex-font-style-bf">in increasing order</span> the indices of the vertices that belong to at least one optimal set.</p>





```input1
5
5 1 3 2 1
1 2
2 3
2 4
1 5
```




```input2
3
1 1 1
1 2
1 3
```




```output1
4 3
2 4 5
```




```output2
2 3
1 2 3
```



## Note

<p>In the second example all sets of two vertices are optimal. So, each vertex is in at least one optimal set.</p>
