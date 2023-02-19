## Description

<div><p>You are given $n$ segments on a number line, numbered from $1$ to $n$. The $i$-th segments covers all integer points from $l_i$ to $r_i$ and has a value $w_i$.</p><p>You are asked to select a subset of these segments (possibly, all of them). Once the subset is selected, it's possible to travel between two integer points if there exists a selected segment that covers both of them. A subset is good if it's possible to reach point $m$ starting from point $1$ in arbitrary number of moves.</p><p>The cost of the subset is the difference between the maximum and the minimum values of segments in it. Find the minimum cost of a good subset.</p><p>In every test there exists at least one good subset.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 3 \cdot 10^5$; $2 \le m \le 10^6$)&nbsp;— the number of segments and the number of integer points.</p><p>Each of the next $n$ lines contains three integers $l_i$, $r_i$ and $w_i$ ($1 \le l_i &lt; r_i \le m$; $1 \le w_i \le 10^6$)&nbsp;— the description of the $i$-th segment.</p><p>In every test there exists at least one good subset.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum cost of a good subset.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 3 \cdot 10^5$; $2 \le m \le 10^6$)&nbsp;— the number of segments and the number of integer points.</p><p>Each of the next $n$ lines contains three integers $l_i$, $r_i$ and $w_i$ ($1 \le l_i &lt; r_i \le m$; $1 \le w_i \le 10^6$)&nbsp;— the description of the $i$-th segment.</p><p>In every test there exists at least one good subset.</p>

## Output

<p>Print a single integer&nbsp;— the minimum cost of a good subset.</p>





```input1
5 12
1 5 5
3 4 10
4 10 6
11 12 5
10 12 3
```




```input2
1 10
1 10 23
```




```output1
3
```




```output2
0
```


