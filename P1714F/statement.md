## Description

<div><p>A tree is a connected undirected graph without cycles. Note that in this problem, we are talking about not rooted trees.</p><p>You are given four positive integers $n, d_{12}, d_{23}$ and $d_{31}$. Construct a tree such that:</p><ul> <li> it contains $n$ vertices numbered from $1$ to $n$, </li><li> the distance (length of the shortest path) from vertex $1$ to vertex $2$ is $d_{12}$, </li><li> distance from vertex $2$ to vertex $3$ is $d_{23}$, </li><li> the distance from vertex $3$ to vertex $1$ is $d_{31}$. </li></ul><p>Output any tree that satisfies all the requirements above, or determine that no such tree exists.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>This is followed by $t$ test cases, each written on a separate line.</p><p>Each test case consists of four positive integers $n, d_{12}, d_{23}$ and $d_{31}$ ($3 \le n \le 2\cdot10^5; 1 \le d_{12}, d_{23}, d_{31} \le n-1$).</p><p>It is guaranteed that the sum of $n$ values for all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if the suitable tree exists, and <span class="tex-font-style-tt">NO</span> otherwise. </p><p>If the answer is positive, print another $n-1$ line each containing a description of an edge of the tree — a pair of positive integers $x_i, y_i$, which means that the $i$th edge connects vertices $x_i$ and $y_i$. </p><p>The edges and vertices of the edges can be printed in any order. If there are several suitable trees, output any of them.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>This is followed by $t$ test cases, each written on a separate line.</p><p>Each test case consists of four positive integers $n, d_{12}, d_{23}$ and $d_{31}$ ($3 \le n \le 2\cdot10^5; 1 \le d_{12}, d_{23}, d_{31} \le n-1$).</p><p>It is guaranteed that the sum of $n$ values for all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if the suitable tree exists, and <span class="tex-font-style-tt">NO</span> otherwise. </p><p>If the answer is positive, print another $n-1$ line each containing a description of an edge of the tree — a pair of positive integers $x_i, y_i$, which means that the $i$th edge connects vertices $x_i$ and $y_i$. </p><p>The edges and vertices of the edges can be printed in any order. If there are several suitable trees, output any of them.</p>





```input1|2,4,6,8,10
9
5 1 2 1
5 2 2 2
5 2 2 3
5 2 2 4
5 3 2 3
4 2 1 1
4 3 1 1
4 1 2 3
7 1 4 1
```




```output1
YES
1 2
4 1
3 1
2 5
YES
4 3
2 5
1 5
5 3
NO
YES
2 4
4 1
2 5
5 3
YES
5 4
4 1
2 5
3 5
YES
2 3
3 4
1 3
NO
YES
4 3
1 2
2 4
NO
```


