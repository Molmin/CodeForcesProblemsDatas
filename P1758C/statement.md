## Description

<div><p>Given two integers $n$ and $x$, a permutation$^{\dagger}$ $p$ of length $n$ is called <span class="tex-font-style-it">funny</span> if $p_i$ is a multiple of $i$ for all $1 \leq i \leq n - 1$, $p_n = 1$, and $p_1 = x$.</p><p>Find the lexicographically minimal$^{\ddagger}$ funny permutation, or report that no such permutation exists.</p><p>$^{\dagger}$ A permutation of length $n$ is an array consisting of each of the integers from $1$ to $n$ exactly once.</p><p>$^{\ddagger}$ Let $a$ and $b$ be permutations of length $n$. Then $a$ is lexicographically smaller than $b$ if in the first position $i$ where $a$ and $b$ differ, $a_i &lt; b_i$. A permutation is lexicographically minimal if it is lexicographically smaller than all other permutations.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $x$ ($2 \leq n \leq 2 \cdot 10^5$; $1 &lt; x \leq n$).</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if the answer exists, output $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \leq p_i \leq n$)&nbsp;— the lexicographically minimal funny permutation $p$. Otherwise, output $-1$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $x$ ($2 \leq n \leq 2 \cdot 10^5$; $1 &lt; x \leq n$).</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, if the answer exists, output $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \leq p_i \leq n$)&nbsp;— the lexicographically minimal funny permutation $p$. Otherwise, output $-1$.</p>





```input1|2,4
3
3 3
4 2
5 4
```




```output1
3 2 1 
2 4 3 1 
-1
```



## Note

<p>In the first test case, the permutation $[3,2,1]$ satisfies all the conditions: $p_1=3$, $p_3=1$, and: </p><ul> <li> $p_1=3$ is a multiple of $1$. </li><li> $p_2=2$ is a multiple of $2$. </li></ul><p>In the second test case, the permutation $[2,4,3,1]$ satisfies all the conditions: $p_1=2$, $p_4=1$, and: </p><ul> <li> $p_1=2$ is a multiple of $1$. </li><li> $p_2=4$ is a multiple of $2$. </li><li> $p_3=3$ is a multiple of $3$. </li></ul><p>We can show that these permutations are lexicographically minimal.</p><p>No such permutations exist in the third test case.</p>
