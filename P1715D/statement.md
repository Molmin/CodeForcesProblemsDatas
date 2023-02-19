## Description

<div><p>The Narrator has an integer array $a$ of length $n$, but he will only tell you the size $n$ and $q$ statements, each of them being three integers $i, j, x$, which means that $a_i \mid a_j = x$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>.</p><p>Find the lexicographically smallest array $a$ that satisfies all the statements.</p><p>An array $a$ is lexicographically smaller than an array $b$ of the same length if and only if the following holds: </p><ul> <li> in the first position where $a$ and $b$ differ, the array $a$ has a smaller element than the corresponding element in $b$. </li></ul></div><div class="input-specification"><p>In the first line you are given with two integers $n$ and $q$ ($1 \le n \le 10^5$, $0 \le q \le 2 \cdot 10^5$).</p><p>In the next $q$ lines you are given with three integers $i$, $j$, and $x$ ($1 \le i, j \le n$, $0 \le x &lt; 2^{30}$)&nbsp;— the statements.</p><p>It is guaranteed that all $q$ statements hold for at least one array.</p></div><div class="output-specification"><p>On a single line print $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;— array $a$.</p></div>

## Input

<p>In the first line you are given with two integers $n$ and $q$ ($1 \le n \le 10^5$, $0 \le q \le 2 \cdot 10^5$).</p><p>In the next $q$ lines you are given with three integers $i$, $j$, and $x$ ($1 \le i, j \le n$, $0 \le x &lt; 2^{30}$)&nbsp;— the statements.</p><p>It is guaranteed that all $q$ statements hold for at least one array.</p>

## Output

<p>On a single line print $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;— array $a$.</p>





```input1
4 3
1 2 3
1 3 2
4 1 2
```




```input2
1 0
```




```input3
2 1
1 1 1073741823
```




```output1
0 3 2 2
```




```output2
0
```




```output3
1073741823 0
```



## Note

<p>In the first sample, these are all the arrays satisfying the statements: </p><ul> <li> $[0, 3, 2, 2]$, </li><li> $[2, 1, 0, 0]$, </li><li> $[2, 1, 0, 2]$, </li><li> $[2, 1, 2, 0]$, </li><li> $[2, 1, 2, 2]$, </li><li> $[2, 3, 0, 0]$, </li><li> $[2, 3, 0, 2]$, </li><li> $[2, 3, 2, 0]$, </li><li> $[2, 3, 2, 2]$. </li></ul>
