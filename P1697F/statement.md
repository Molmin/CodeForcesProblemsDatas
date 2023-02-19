## Description

<div><p>You are asked to build an array $a$, consisting of $n$ integers, each element should be from $1$ to $k$.</p><p>The array should be non-decreasing ($a_i \le a_{i+1}$ for all $i$ from $1$ to $n-1$). </p><p>You are also given additional constraints on it. Each constraint is of one of three following types: </p><ul> <li> $1~i~x$: $a_i$ <span class="tex-font-style-bf">should not</span> be equal to $x$; </li><li> $2~i~j~x$: $a_i + a_j$ should be less than or equal to $x$; </li><li> $3~i~j~x$: $a_i + a_j$ should be greater than or equal to $x$. </li></ul><p>Build any non-decreasing array that satisfies all constraints or report that no such array exists.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains three integers $n, m$ and $k$ ($2 \le n \le 2 \cdot 10^4$; $0 \le m \le 2 \cdot 10^4$; $2 \le k \le 10$).</p><p>The $i$-th of the next $m$ lines contains a description of a constraint. Each constraint is of one of three following types: </p><ul> <li> $1~i~x$ ($1 \le i \le n$; $1 \le x \le k$): $a_i$ <span class="tex-font-style-bf">should not</span> be equal to $x$; </li><li> $2~i~j~x$ ($1 \le i &lt; j \le n$; $2 \le x \le 2 \cdot k$): $a_i + a_j$ should be less than or equal to $x$; </li><li> $3~i~j~x$ ($1 \le i &lt; j \le n$; $2 \le x \le 2 \cdot k$): $a_i + a_j$ should be greater than or equal to $x$. </li></ul><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^4$. The sum of $m$ over all testcases doesn't exceed $2 \cdot 10^4$.</p></div><div class="output-specification"><p>For each testcase, determine if there exists a non-decreasing array that satisfies all conditions. If there is no such array, then print <span class="tex-font-style-tt">-1</span>. Otherwise, print any valid array&nbsp;— $n$ integers from $1$ to $k$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains three integers $n, m$ and $k$ ($2 \le n \le 2 \cdot 10^4$; $0 \le m \le 2 \cdot 10^4$; $2 \le k \le 10$).</p><p>The $i$-th of the next $m$ lines contains a description of a constraint. Each constraint is of one of three following types: </p><ul> <li> $1~i~x$ ($1 \le i \le n$; $1 \le x \le k$): $a_i$ <span class="tex-font-style-bf">should not</span> be equal to $x$; </li><li> $2~i~j~x$ ($1 \le i &lt; j \le n$; $2 \le x \le 2 \cdot k$): $a_i + a_j$ should be less than or equal to $x$; </li><li> $3~i~j~x$ ($1 \le i &lt; j \le n$; $2 \le x \le 2 \cdot k$): $a_i + a_j$ should be greater than or equal to $x$. </li></ul><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^4$. The sum of $m$ over all testcases doesn't exceed $2 \cdot 10^4$.</p>

## Output

<p>For each testcase, determine if there exists a non-decreasing array that satisfies all conditions. If there is no such array, then print <span class="tex-font-style-tt">-1</span>. Otherwise, print any valid array&nbsp;— $n$ integers from $1$ to $k$.</p>





```input1
4
4 0 4
2 2 3
3 1 2 3
1 2 2
3 3 2
1 1 1
2 2 3 2
3 2 3 2
5 5 5
3 2 5 7
2 4 5 10
3 4 5 6
3 3 4 7
2 1 5 7
```




```output1
1 2 3 4
1 3
-1
1 2 2 5 5
```


