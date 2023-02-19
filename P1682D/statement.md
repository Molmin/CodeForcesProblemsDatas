## Description

<div><p>There are $n$ nodes arranged in a circle numbered from $1$ to $n$ in the clockwise order. You are also given a binary string $s$ of length $n$.</p><p>Your task is to construct a tree on the given $n$ nodes satisfying the two conditions below or report that there such tree does not exist:</p><ul> <li> For each node $i$ $(1 \le i \le n)$, the degree of node is even if $s_i = 0$ and odd if $s_i = 1$. </li><li> No two edges of the tree intersect internally in the circle. The edges are allowed to intersect on the circumference. </li></ul> <p>Note that all edges are drawn as straight line segments. For example, edge $(u, v)$ in the tree is drawn as a line segment connecting $u$ and $v$ on the circle.</p><p>A tree on $n$ nodes is a connected graph with $n - 1$ edges.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 2\cdot 10^4)$ &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \leq n \leq 2\cdot 10^5)$ &nbsp;— the number of nodes.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if there does not exist a tree that satisfies the given conditions, then output "<span class="tex-font-style-tt">NO</span>" (without quotes), otherwise output "<span class="tex-font-style-tt">YES</span>" followed by the description of tree.</p><p>You can output each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yEs</span>" will be recognized as a positive answer).</p><p>If there exists a tree, then output $n - 1$ lines, each containing two integers $u$ and $v$ $(1 \leq u,v \leq n, u \neq v)$ denoting an edge between $u$ and $v$ in the tree. If there are multiple possible answers, output any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 2\cdot 10^4)$ &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \leq n \leq 2\cdot 10^5)$ &nbsp;— the number of nodes.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, if there does not exist a tree that satisfies the given conditions, then output "<span class="tex-font-style-tt">NO</span>" (without quotes), otherwise output "<span class="tex-font-style-tt">YES</span>" followed by the description of tree.</p><p>You can output each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yEs</span>" will be recognized as a positive answer).</p><p>If there exists a tree, then output $n - 1$ lines, each containing two integers $u$ and $v$ $(1 \leq u,v \leq n, u \neq v)$ denoting an edge between $u$ and $v$ in the tree. If there are multiple possible answers, output any.</p>





```input1
3
4
0110
2
10
6
110110
```




```output1
YES
2 1
3 4
1 4
NO
YES
2 3
1 2
5 6
6 2
3 4
```



## Note

<p>In the first test case, the tree looks as follows: </p><center> <img class="tex-graphics" src="file://CfzeSygG.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>In the second test case, there is only one possible tree with an edge between $1$ and $2$, and it does not satisfy the degree constraints.</p><p>In the third test case, </p><center> <img class="tex-graphics" src="file://yl1tkgAs.png" style="max-width: 100.0%;max-height: 100.0%;" width="1512px"> </center> The tree on the left satisfies the degree constraints but the edges intersect internally, therefore it is not a valid tree, while the tree on the right is valid.
