## Description

<div><p>We say an infinite sequence $a_{0}, a_{1}, a_2, \ldots$ is <span class="tex-font-style-bf">non-increasing</span> if and only if for all $i\ge 0$, $a_i \ge a_{i+1}$.</p><p>There is an infinite right and down grid. The upper-left cell has coordinates $(0,0)$. Rows are numbered $0$ to infinity from top to bottom, columns are numbered from $0$ to infinity from left to right.</p><p>There is also a <span class="tex-font-style-bf">non-increasing</span> infinite sequence $a_{0}, a_{1}, a_2, \ldots$. You are given $a_0$, $a_1$, $\ldots$, $a_n$; for all $i&gt;n$, $a_i=0$. For every pair of $x$, $y$, the cell with coordinates $(x,y)$ (which is located at the intersection of $x$-th row and $y$-th column) is white if $y&lt;a_x$ and black otherwise.</p><p>Initially there is one doll named Jina on $(0,0)$. You can do the following operation.</p><ul> <li> Select one doll on $(x,y)$. Remove it and place a doll on $(x,y+1)$ and place a doll on $(x+1,y)$. </li></ul><p>Note that multiple dolls can be present at a cell at the same time; in one operation, you remove only one. Your goal is to make all white cells contain $0$ dolls.</p><p>What's the minimum number of operations needed to achieve the goal? Print the answer modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line of input contains one integer $n$ ($1\le n\le 2\cdot 10^5$).</p><p>The second line of input contains $n+1$ integers $a_0,a_1,\ldots,a_n$ ($0\le a_i\le 2\cdot 10^5$).</p><p>It is guaranteed that the sequence $a$ is <span class="tex-font-style-bf">non-increasing</span>.</p></div><div class="output-specification"><p>Print one integer — the answer to the problem, modulo $10^9+7$.</p></div>

## Input

<p>The first line of input contains one integer $n$ ($1\le n\le 2\cdot 10^5$).</p><p>The second line of input contains $n+1$ integers $a_0,a_1,\ldots,a_n$ ($0\le a_i\le 2\cdot 10^5$).</p><p>It is guaranteed that the sequence $a$ is <span class="tex-font-style-bf">non-increasing</span>.</p>

## Output

<p>Print one integer — the answer to the problem, modulo $10^9+7$.</p>





```input1
2
2 2 0
```




```input2
10
12 11 8 8 6 6 6 5 3 2 1
```




```output1
5
```




```output2
2596
```



## Note

<p>Consider the first example. In the given grid, cells $(0,0),(0,1),(1,0),(1,1)$ are white, and all other cells are black. Let us use triples to describe the grid: triple $(x,y,z)$ means that there are $z$ dolls placed on cell $(x,y)$. Initially the state of the grid is $(0,0,1)$.</p><p>One of the optimal sequence of operations is as follows:</p><ul> <li> Do the operation with $(0,0)$. Now the state of the grid is $(1,0,1),(0,1,1)$. </li><li> Do the operation with $(0,1)$. Now the state of the grid is $(1,0,1),(1,1,1),(0,2,1)$. </li><li> Do the operation with $(1,0)$. Now the state of the grid is $(1,1,2),(0,2,1),(2,0,1)$. </li><li> Do the operation with $(1,1)$. Now the state of the grid is $(1,1,1),(0,2,1),(2,0,1),(1,2,1),(2,1,1)$. </li><li> Do the operation with $(1,1)$. Now the state of the grid is $(0,2,1),(2,0,1),(1,2,2),(2,1,2)$. </li></ul><p>Now all white cells contain $0$ dolls, so we have achieved the goal with $5$ operations.</p>
