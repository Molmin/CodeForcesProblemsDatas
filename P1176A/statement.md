## Description

<div><p>You are given an integer $n$.</p><p>You can perform any of the following operations with this number an arbitrary (possibly, zero) number of times: </p><ol> <li> Replace $n$ with $\frac{n}{2}$ if $n$ is divisible by $2$; </li><li> Replace $n$ with $\frac{2n}{3}$ if $n$ is divisible by $3$; </li><li> Replace $n$ with $\frac{4n}{5}$ if $n$ is divisible by $5$. </li></ol><p>For example, you can replace $30$ with $15$ using the first operation, with $20$ using the second operation or with $24$ using the third operation.</p><p>Your task is to find the minimum number of moves required to obtain $1$ from $n$ or say that it is impossible to do it.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 1000$) — the number of queries.</p><p>The next $q$ lines contain the queries. For each query you are given the integer number $n$ ($1 \le n \le 10^{18}$).</p></div><div class="output-specification"><p>Print the answer for each query on a new line. If it is impossible to obtain $1$ from $n$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum number of moves required to do it.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 1000$) — the number of queries.</p><p>The next $q$ lines contain the queries. For each query you are given the integer number $n$ ($1 \le n \le 10^{18}$).</p>

## Output

<p>Print the answer for each query on a new line. If it is impossible to obtain $1$ from $n$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum number of moves required to do it.</p>





```input1
7
1
10
25
30
14
27
1000000000000000000
```




```output1
0
4
6
6
-1
6
72
```


