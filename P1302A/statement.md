## Description

<div><p><span class="tex-font-style-it">This is an unusual problem in an unusual contest, here is the announcement: <a href="//codeforces.com/blog/entry/73543">http://codeforces.com/blog/entry/73543</a></span></p><p>You are given a table $A$ of integers $n \times m$. The cell $(x, y)$ is called <span class="tex-font-style-it">Nash equilibrium</span> if both of the following conditions hold: </p><ul> <li> for each $x_1 \neq x$ $A_{xy} &gt; A_{x_1y}$; </li><li> for each $y_1 \neq y$ $A_{xy} &lt; A_{xy_1}$. </li></ul><p>Find a Nash equilibrium in $A$. If there exist several equilibria, print the one with minimum $x$. If still there are several possible answers, print the one with minimum $y$.</p></div><div class="input-specification"><p>The first line contains two integers $n, m$ ($2 \leq n, m \leq 1000$), denoting the size of the table.</p><p>Each of next $n$ lines contain $m$ space-separated integers $A_{ij}$ ($1 \leq A_{ij} \leq 10^9$).</p></div><div class="output-specification"><p>Output $x$ and $y$ — the coordinates of the lexicographically minimum Nash equilibrium in the table. In case there is no answer, print two zeroes instead.</p></div>

## Input

<p>The first line contains two integers $n, m$ ($2 \leq n, m \leq 1000$), denoting the size of the table.</p><p>Each of next $n$ lines contain $m$ space-separated integers $A_{ij}$ ($1 \leq A_{ij} \leq 10^9$).</p>

## Output

<p>Output $x$ and $y$ — the coordinates of the lexicographically minimum Nash equilibrium in the table. In case there is no answer, print two zeroes instead.</p>





```input1
4 4
1 2 3 4
1 2 3 5
1 2 3 6
2 3 5 7
```




```input2
3 5
7 7 7 7 7
7 7 7 7 7
7 7 7 7 7
```




```output1
1 4
```




```output2
0 0
```


