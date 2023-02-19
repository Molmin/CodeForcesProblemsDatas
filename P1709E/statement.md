## Description

<div><p>You are given a tree consisting of $n$ vertices. A number is written on each vertex; the number on vertex $i$ is equal to $a_i$.</p><p>Recall that a simple path is a path that visits each vertex at most once. Let the <span class="tex-font-style-it">weight</span> of the path be the bitwise XOR of the values written on vertices it consists of. Let's say that a tree is <span class="tex-font-style-it">good</span> if no simple path has weight $0$.</p><p>You can apply the following operation any number of times (possibly, zero): select a vertex of the tree and replace the value written on it with an arbitrary positive integer. What is the minimum number of times you have to apply this operation in order to make the tree <span class="tex-font-style-it">good</span>?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i &lt; 2^{30}$)&nbsp;— the numbers written on vertices.</p><p>Then $n - 1$ lines follow, each containing two integers $x$ and $y$ ($1 \le x, y \le n; x \ne y$) denoting an edge connecting vertex $x$ with vertex $y$. It is guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of times you have to apply the operation in order to make the tree <span class="tex-font-style-it">good</span>.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i &lt; 2^{30}$)&nbsp;— the numbers written on vertices.</p><p>Then $n - 1$ lines follow, each containing two integers $x$ and $y$ ($1 \le x, y \le n; x \ne y$) denoting an edge connecting vertex $x$ with vertex $y$. It is guaranteed that these edges form a tree.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of times you have to apply the operation in order to make the tree <span class="tex-font-style-it">good</span>.</p>





```input1
6
3 2 1 3 2 1
4 5
3 4
1 4
2 1
6 1
```




```input2
4
2 1 1 1
1 2
1 3
1 4
```




```input3
5
2 2 2 2 2
1 2
2 3
3 4
4 5
```




```output1
2
```




```output2
0
```




```output3
2
```



## Note

<p>In the first example, it is enough to replace the value on the vertex $1$ with $13$, and the value on the vertex $4$ with $42$.</p>
