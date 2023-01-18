## Description

<div><p>Consider the infinite sequence $s$ of positive integers, created by repeating the following steps:</p><ol> <li> Find the lexicographically smallest triple of positive integers $(a, b, c)$ such that <ul> <li> $a \oplus b \oplus c = 0$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </li><li> $a$, $b$, $c$ are not in $s$. </li></ul> Here triple of integers $(a_1, b_1, c_1)$ is considered to be lexicographically smaller than triple $(a_2, b_2, c_2)$ if sequence $[a_1, b_1, c_1]$ is lexicographically smaller than sequence $[a_2, b_2, c_2]$. </li><li> Append $a$, $b$, $c$ to $s$ in this order. </li><li> Go back to the first step. </li></ol><p>You have integer $n$. Find the $n$-th element of $s$.</p><p>You have to answer $t$ independent test cases.</p><p>A sequence $a$ is lexicographically smaller than a sequence $b$ if in the first position where $a$ and $b$ differ, the sequence $a$ has a smaller element than the corresponding element in $b$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>Each of the next $t$ lines contains a single integer $n$ ($1\le n \le 10^{16}$)&nbsp;— the position of the element you want to know.</p></div><div class="output-specification"><p>In each of the $t$ lines, output the answer to the corresponding test case.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>Each of the next $t$ lines contains a single integer $n$ ($1\le n \le 10^{16}$)&nbsp;— the position of the element you want to know.</p>

## Output

<p>In each of the $t$ lines, output the answer to the corresponding test case.</p>





```input1
9
1
2
3
4
5
6
7
8
9
```




```output1
1
2
3
4
8
12
5
10
15
```



## Note

<p>The first elements of $s$ are $1, 2, 3, 4, 8, 12, 5, 10, 15, \dots $</p>
