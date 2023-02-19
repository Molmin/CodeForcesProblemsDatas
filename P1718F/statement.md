## Description

<div><p>Eugene got Burenka an array $a$ of length $n$ of integers from $1$ to $m$ for her birthday. Burenka knows that Eugene really likes <span class="tex-font-style-it">coprime</span> integers (integers $x$ and $y$ such that they have only one common factor (equal to $1$)) so she wants to to ask Eugene $q$ questions about the present. </p><p>Each time Burenka will choose a subsegment $a_l, a_{l + 1}, \ldots, a_r$ of array $a$, and compute the product of these numbers $p = a_l \cdot a_{l + 1} \cdot \ldots \cdot a_r$. Then she will ask Eugene to count the number of integers between $1$ and $C$ inclusive which are coprime with $p$. </p><p>Help Eugene answer all the questions!</p></div><div class="input-specification"><p>In the first line of input there are four integers $n$, $m$, $C$, $q$ ($1 \leq n, q \leq 10^5$, $1 \leq m \leq 2\cdot 10^4$, $1 \leq C \leq 10^5$)&nbsp;— the length of the array $a$, the maximum possible value of $a_{i}$, the value $C$, and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_{i} \leq m$)&nbsp;— the array $a$ .</p><p>In the next $q$ lines the queries are given. Each query consists of two integers $l$ and $r$ ($1 \leq l \leq r \leq n$).</p></div><div class="output-specification"><p>Print $q$ integers&nbsp;— the answers to Burenka's queries.</p></div>

## Input

<p>In the first line of input there are four integers $n$, $m$, $C$, $q$ ($1 \leq n, q \leq 10^5$, $1 \leq m \leq 2\cdot 10^4$, $1 \leq C \leq 10^5$)&nbsp;— the length of the array $a$, the maximum possible value of $a_{i}$, the value $C$, and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_{i} \leq m$)&nbsp;— the array $a$ .</p><p>In the next $q$ lines the queries are given. Each query consists of two integers $l$ and $r$ ($1 \leq l \leq r \leq n$).</p>

## Output

<p>Print $q$ integers&nbsp;— the answers to Burenka's queries.</p>





```input1
5 5 5 3
1 2 3 2 5
1 1
2 4
4 5
```




```output1
5
2
2
```



## Note

<p>Here's an explanation for the example:</p><ol> <li> in the first query, the product is equal to $1$, which is coprime with $1,2,3,4,5$. </li><li> in the second query, the product is equal to $12$, which is coprime with $1$ and $5$. </li><li> in the third query, the product is equal to $10$, which is coprime with $1$ and $3$. </li></ol>
