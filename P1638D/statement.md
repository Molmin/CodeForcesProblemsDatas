## Description

<div><p>You found a painting on a canvas of size $n \times m$. The canvas can be represented as a grid with $n$ rows and $m$ columns. Each cell has some color. Cell $(i, j)$ has color $c_{i,j}$.</p><p>Near the painting you also found a brush in the shape of a $2 \times 2$ square, so the canvas was surely painted in the following way: initially, no cell was painted. Then, the following painting operation has been performed some number of times:</p><ul> <li> Choose two integers $i$ and $j$ ($1 \le i &lt; n$, $1 \le j &lt; m$) and some color $k$ ($1 \le k \le nm$). </li><li> Paint cells $(i, j)$, $(i + 1, j)$, $(i, j + 1)$, $(i + 1, j + 1)$ in color $k$. </li></ul><p>All cells must be painted at least once. A cell can be painted multiple times. In this case, its final color will be the last one.</p><p>Find any sequence of at most $nm$ operations that could have led to the painting you found or state that it's impossible.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $m$ ($2 \le n, m \le 1000$)&nbsp;— the dimensions of the canvas.</p><p>On the $i$-th of the next $n$ lines of input, there will be $m$ integers. The $j$-th of them is $a_{i,j}$ ($1 \le a_{i,j} \le nm$) — the color of cell $(i, j)$.</p></div><div class="output-specification"><p>If there is no solution, print a single integer $-1$.</p><p>Otherwise, on the first line, print one integer $q$ ($1 \le q \le nm$)&nbsp;— the number of operations.</p><p>Next, print the operations in order. On the $k$-th of the next $q$ lines, print three integers $i$, $j$, $c$ ($1 \le i &lt; n$, $1 \le j &lt; m$, $1 \le c \le nm$)&nbsp;— the description of the $k$-th operation.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $m$ ($2 \le n, m \le 1000$)&nbsp;— the dimensions of the canvas.</p><p>On the $i$-th of the next $n$ lines of input, there will be $m$ integers. The $j$-th of them is $a_{i,j}$ ($1 \le a_{i,j} \le nm$) — the color of cell $(i, j)$.</p>

## Output

<p>If there is no solution, print a single integer $-1$.</p><p>Otherwise, on the first line, print one integer $q$ ($1 \le q \le nm$)&nbsp;— the number of operations.</p><p>Next, print the operations in order. On the $k$-th of the next $q$ lines, print three integers $i$, $j$, $c$ ($1 \le i &lt; n$, $1 \le j &lt; m$, $1 \le c \le nm$)&nbsp;— the description of the $k$-th operation.</p><p>If there are multiple solutions, print any.</p>





```input1
4 4
5 5 3 3
1 1 5 3
2 2 5 4
2 2 4 4
```




```input2
3 4
1 1 1 1
2 2 3 1
2 2 1 1
```




```output1
6
1 3 3
3 3 4
2 2 5
1 1 5
2 1 1
3 1 2
```




```output2
-1
```



## Note

<p>In the first test case, the solution is not unique. Here's one of them:</p><center> <img class="tex-graphics" src="file://FioBsrYg.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>In the second test case, there is no way one could obtain the given painting, thus the answer is $-1$.</p>
