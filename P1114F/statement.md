## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$.</p><p>You need to perform $q$ queries of the following two types:</p><ol> <li> "<span class="tex-font-style-tt">MULTIPLY l r x</span>"&nbsp;— for every $i$ ($l \le i \le r$) multiply $a_i$ by $x$.</li><li> "<span class="tex-font-style-tt">TOTIENT l r</span>"&nbsp;— print $\varphi(\prod \limits_{i=l}^{r} a_i)$ taken modulo $10^9+7$, where $\varphi$ denotes Euler's totient function. </li></ol><p>The <a href="http://gg.gg/euler_totient">Euler's totient function</a> of a positive integer $n$ (denoted as $\varphi(n)$) is the number of integers $x$ ($1 \le x \le n$) such that $\gcd(n,x) = 1$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n \le 4 \cdot 10^5$, $1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of elements in array $a$ and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 300$)&nbsp;— the elements of array $a$.</p><p>Then $q$ lines follow, describing queries in the format given in the statement.</p><ol> <li> "<span class="tex-font-style-tt">MULTIPLY l r x</span>" ($1 \le l \le r \le n$, $1 \le x \le 300$)&nbsp;— denotes a multiplication query.</li><li> "<span class="tex-font-style-tt">TOTIENT l r</span>" ($1 \le l \le r \le n$)&nbsp;— denotes a query on the value of Euler's totient function. </li></ol><p>It is guaranteed that there is at least one "<span class="tex-font-style-tt">TOTIENT</span>" query.</p></div><div class="output-specification"><p>For each "<span class="tex-font-style-tt">TOTIENT</span>" query, print the answer to it.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n \le 4 \cdot 10^5$, $1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of elements in array $a$ and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 300$)&nbsp;— the elements of array $a$.</p><p>Then $q$ lines follow, describing queries in the format given in the statement.</p><ol> <li> "<span class="tex-font-style-tt">MULTIPLY l r x</span>" ($1 \le l \le r \le n$, $1 \le x \le 300$)&nbsp;— denotes a multiplication query.</li><li> "<span class="tex-font-style-tt">TOTIENT l r</span>" ($1 \le l \le r \le n$)&nbsp;— denotes a query on the value of Euler's totient function. </li></ol><p>It is guaranteed that there is at least one "<span class="tex-font-style-tt">TOTIENT</span>" query.</p>

## Output

<p>For each "<span class="tex-font-style-tt">TOTIENT</span>" query, print the answer to it.</p>





```input1
4 4
5 9 1 2
TOTIENT 3 3
TOTIENT 3 4
MULTIPLY 4 4 3
TOTIENT 4 4

```




```output1
1
1
2

```



## Note

<p>In the first example, $\varphi(1) = 1$ for the first query, $\varphi(2) = 1$ for the second query and $\varphi(6) = 2$ for the third one.</p>
