## Description

<div><p>We say that a positive integer $n$ is $k$-good for some positive integer $k$ if $n$ can be expressed as a sum of $k$ positive integers which give $k$ distinct remainders when divided by $k$.</p><p>Given a positive integer $n$, find some $k \geq 2$ so that $n$ is $k$-good or tell that such a $k$ does not exist.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases.</p><p>Each test case consists of one line with an integer $n$ ($2 \leq n \leq 10^{18}$).</p></div><div class="output-specification"><p>For each test case, print a line with a value of $k$ such that $n$ is $k$-good ($k \geq 2$), or $-1$ if $n$ is not $k$-good for any $k$. If there are multiple valid values of $k$, you can print any of them.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases.</p><p>Each test case consists of one line with an integer $n$ ($2 \leq n \leq 10^{18}$).</p>

## Output

<p>For each test case, print a line with a value of $k$ such that $n$ is $k$-good ($k \geq 2$), or $-1$ if $n$ is not $k$-good for any $k$. If there are multiple valid values of $k$, you can print any of them.</p>





```input1
5
2
4
6
15
20
```




```output1
-1
-1
3
3
5
```



## Note

<p>$6$ is a $3$-good number since it can be expressed as a sum of $3$ numbers which give different remainders when divided by $3$: $6 = 1 + 2 + 3$.</p><p>$15$ is also a $3$-good number since $15 = 1 + 5 + 9$ and $1, 5, 9$ give different remainders when divided by $3$.</p><p>$20$ is a $5$-good number since $20 = 2 + 3 + 4 + 5 + 6$ and $2,3,4,5,6$ give different remainders when divided by $5$.</p>
