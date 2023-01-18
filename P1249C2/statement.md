## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is the maximum value of $n$</span>.</p><p>You are given a positive integer number $n$. You really love <span class="tex-font-style-it">good numbers</span> so you want to find the smallest <span class="tex-font-style-it">good number</span> greater than or equal to $n$.</p><p>The positive integer is called <span class="tex-font-style-it">good</span> if it can be represented as a sum of <span class="tex-font-style-bf">distinct</span> powers of $3$ (i.e. no duplicates of powers of $3$ are allowed).</p><p>For example:</p><ul> <li> $30$ is a <span class="tex-font-style-it">good number</span>: $30 = 3^3 + 3^1$, </li><li> $1$ is a <span class="tex-font-style-it">good number</span>: $1 = 3^0$, </li><li> $12$ is a <span class="tex-font-style-it">good number</span>: $12 = 3^2 + 3^1$, </li><li> but $2$ is <span class="tex-font-style-bf">not</span> a <span class="tex-font-style-it">good number</span>: you can't represent it as a sum of distinct powers of $3$ ($2 = 3^0 + 3^0$), </li><li> $19$ is <span class="tex-font-style-bf">not</span> a <span class="tex-font-style-it">good number</span>: you can't represent it as a sum of distinct powers of $3$ (for example, the representations $19 = 3^2 + 3^2 + 3^0 = 3^2 + 3^1 + 3^1 + 3^1 + 3^0$ are invalid), </li><li> $20$ is also <span class="tex-font-style-bf">not</span> a <span class="tex-font-style-it">good number</span>: you can't represent it as a sum of distinct powers of $3$ (for example, the representation $20 = 3^2 + 3^2 + 3^0 + 3^0$ is invalid). </li></ul><p>Note, that there exist other representations of $19$ and $20$ as sums of powers of $3$ but none of them consists of <span class="tex-font-style-bf">distinct</span> powers of $3$.</p><p>For the given positive integer $n$ find such smallest $m$ ($n \le m$) that $m$ is a <span class="tex-font-style-it">good number</span>.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 500$) — the number of queries. Then $q$ queries follow.</p><p>The only line of the query contains one integer $n$ ($1 \le n \le 10^{18}$).</p></div><div class="output-specification"><p>For each query, print such smallest integer $m$ (where $n \le m$) that $m$ is a <span class="tex-font-style-it">good number</span>.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 500$) — the number of queries. Then $q$ queries follow.</p><p>The only line of the query contains one integer $n$ ($1 \le n \le 10^{18}$).</p>

## Output

<p>For each query, print such smallest integer $m$ (where $n \le m$) that $m$ is a <span class="tex-font-style-it">good number</span>.</p>





```input1
8
1
2
6
13
14
3620
10000
1000000000000000000
```




```output1
1
3
9
13
27
6561
19683
1350851717672992089
```


