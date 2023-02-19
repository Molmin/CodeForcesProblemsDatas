## Description

<div><p>For two positive integers $l$ and $r$ ($l \le r$) let $c(l, r)$ denote the number of integer pairs $(i, j)$ such that $l \le i \le j \le r$ and $\operatorname{gcd}(i, j) \ge l$. Here, $\operatorname{gcd}(i, j)$ is the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $i$ and $j$.</p><p>YouKn0wWho has two integers $n$ and $k$ where $1 \le k \le n$. Let $f(n, k)$ denote the minimum of $\sum\limits_{i=1}^{k}{c(x_i+1,x_{i+1})}$ over all integer sequences $0=x_1 \lt x_2 \lt \ldots \lt x_{k} \lt x_{k+1}=n$.</p><p>Help YouKn0wWho find $f(n, k)$. </p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^5$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$). </p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— $f(n, k)$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^5$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$). </p>

## Output

<p>For each test case, print a single integer&nbsp;— $f(n, k)$.</p>





```input1
4
6 2
4 4
3 1
10 3
```




```output1
8
4
6
11
```



## Note

<p>In the first test case, YouKn0wWho can select the sequence $[0, 2, 6]$. So $f(6, 2) = c(1, 2) + c(3, 6) = 3 + 5 = 8$ which is the minimum possible.</p>
