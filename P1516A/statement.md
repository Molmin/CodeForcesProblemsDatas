## Description

<div><p>Given an array $a$ of length $n$, you can do at most $k$ operations of the following type on it:</p><ul> <li> choose $2$ different elements in the array, add $1$ to the first, and subtract $1$ from the second. However, all the elements of $a$ have to remain non-negative after this operation. </li></ul><p>What is lexicographically the smallest array you can obtain?</p><p>An array $x$ is <a href="https://en.wikipedia.org/wiki/Lexicographical_order">lexicographically smaller</a> than an array $y$ if there exists an index $i$ such that $x_i&lt;y_i$, and $x_j=y_j$ for all $1 \le j &lt; i$. Less formally, at the first index $i$ in which they differ, $x_i&lt;y_i$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 20$)&nbsp;– the number of test cases you need to solve.</p><p>The first line of each test case contains $2$ integers $n$ and $k$ ($2 \le n \le 100$, $1 \le k \le 10000$)&nbsp;— the number of elements in the array and the maximum number of operations you can make.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($0 \le a_i \le 100$)&nbsp;— the elements of the array $a$.</p></div><div class="output-specification"><p>For each test case, print the lexicographically smallest array you can obtain after at most $k$ operations.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 20$)&nbsp;– the number of test cases you need to solve.</p><p>The first line of each test case contains $2$ integers $n$ and $k$ ($2 \le n \le 100$, $1 \le k \le 10000$)&nbsp;— the number of elements in the array and the maximum number of operations you can make.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($0 \le a_i \le 100$)&nbsp;— the elements of the array $a$.</p>

## Output

<p>For each test case, print the lexicographically smallest array you can obtain after at most $k$ operations.</p>





```input1
2
3 1
3 1 4
2 10
1 0
```




```output1
2 1 5 
0 1
```



## Note

<p>In the second test case, we start by subtracting $1$ from the first element and adding $1$ to the second. Then, we can't get any lexicographically smaller arrays, because we can't make any of the elements negative.</p>
