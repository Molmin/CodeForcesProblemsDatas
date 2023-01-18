## Description

<div><p>You are given $n$ positive integers $a_1, \ldots, a_n$, and an integer $k \geq 2$. Count the number of pairs $i, j$ such that $1 \leq i &lt; j \leq n$, and there exists an integer $x$ such that $a_i \cdot a_j = x^k$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \leq n \leq 10^5$, $2 \leq k \leq 100$).</p><p>The second line contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq 10^5$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of suitable pairs.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \leq n \leq 10^5$, $2 \leq k \leq 100$).</p><p>The second line contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq 10^5$).</p>

## Output

<p>Print a single integer&nbsp;— the number of suitable pairs.</p>





```input1
6 3
1 3 9 8 24 1
```




```output1
5
```



## Note

<p>In the sample case, the suitable pairs are:</p><ul><li> $a_1 \cdot a_4 = 8 = 2^3$;</li><li> $a_1 \cdot a_6 = 1 = 1^3$;</li><li> $a_2 \cdot a_3 = 27 = 3^3$;</li><li> $a_3 \cdot a_5 = 216 = 6^3$;</li><li> $a_4 \cdot a_6 = 8 = 2^3$.</li></ul>
