## Description

<div><p>You are given $n$ elements numbered from $1$ to $n$, the element $i$ has value $a_i$ and color $c_i$, initially, $c_i = 0$ for all $i$.</p><p>The following operation can be applied:</p><ul> <li> Select three elements $i$, $j$ and $k$ ($1 \leq i &lt; j &lt; k \leq n$), such that $c_i$, $c_j$ and $c_k$ are all equal to $0$ and $a_i = a_k$, then set $c_j = 1$. </li></ul><p>Find the maximum value of $\sum\limits_{i=1}^n{c_i}$ that can be obtained after applying the given operation any number of times.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$) — the number of elements.</p><p>The second line consists of $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$), where $a_i$ is the value of the $i$-th element.</p></div><div class="output-specification"><p>Print a single integer in a line — the maximum value of $\sum\limits_{i=1}^n{c_i}$ that can be obtained after applying the given operation any number of times.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$) — the number of elements.</p><p>The second line consists of $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$), where $a_i$ is the value of the $i$-th element.</p>

## Output

<p>Print a single integer in a line — the maximum value of $\sum\limits_{i=1}^n{c_i}$ that can be obtained after applying the given operation any number of times.</p>





```input1
7
1 2 1 2 7 4 7
```




```input2
13
1 2 3 2 1 3 3 4 5 5 5 4 7
```




```output1
2
```




```output2
7
```



## Note

<p>In the first test, it is possible to apply the following operations in order:</p><center> <img class="tex-graphics" src="file://95AYvwMQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
