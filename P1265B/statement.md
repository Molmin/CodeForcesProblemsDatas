## Description

<div><p>You are given a permutation $p=[p_1, p_2, \ldots, p_n]$ of integers from $1$ to $n$. Let's call the number $m$ ($1 \le m \le n$) <span class="tex-font-style-it">beautiful</span>, if there exists two indices $l, r$ ($1 \le l \le r \le n$), such that the numbers $[p_l, p_{l+1}, \ldots, p_r]$ is a permutation of numbers $1, 2, \ldots, m$.</p><p>For example, let $p = [4, 5, 1, 3, 2, 6]$. In this case, the numbers $1, 3, 5, 6$ are beautiful and $2, 4$ are not. It is because:</p><ul> <li> if $l = 3$ and $r = 3$ we will have a permutation $[1]$ for $m = 1$; </li><li> if $l = 3$ and $r = 5$ we will have a permutation $[1, 3, 2]$ for $m = 3$; </li><li> if $l = 1$ and $r = 5$ we will have a permutation $[4, 5, 1, 3, 2]$ for $m = 5$; </li><li> if $l = 1$ and $r = 6$ we will have a permutation $[4, 5, 1, 3, 2, 6]$ for $m = 6$; </li><li> it is impossible to take some $l$ and $r$, such that $[p_l, p_{l+1}, \ldots, p_r]$ is a permutation of numbers $1, 2, \ldots, m$ for $m = 2$ and for $m = 4$. </li></ul><p>You are given a permutation $p=[p_1, p_2, \ldots, p_n]$. For all $m$ ($1 \le m \le n$) determine if it is a beautiful number or not.</p></div><div class="input-specification"><p>The first line contains the only integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases in the input. The next lines contain the description of test cases.</p><p>The first line of a test case contains a number $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the given permutation $p$. The next line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, all $p_i$ are different)&nbsp;— the given permutation $p$.</p><p>It is guaranteed, that the sum of $n$ from all test cases in the input doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ lines&nbsp;— the answers to test cases in the order they are given in the input. </p><p>The answer to a test case is the string of length $n$, there the $i$-th character is equal to $1$ if $i$ is a beautiful number and is equal to $0$ if $i$ is not a beautiful number.</p></div>

## Input

<p>The first line contains the only integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases in the input. The next lines contain the description of test cases.</p><p>The first line of a test case contains a number $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the given permutation $p$. The next line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, all $p_i$ are different)&nbsp;— the given permutation $p$.</p><p>It is guaranteed, that the sum of $n$ from all test cases in the input doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $t$ lines&nbsp;— the answers to test cases in the order they are given in the input. </p><p>The answer to a test case is the string of length $n$, there the $i$-th character is equal to $1$ if $i$ is a beautiful number and is equal to $0$ if $i$ is not a beautiful number.</p>





```input1
3
6
4 5 1 3 2 6
5
5 3 1 2 4
4
1 4 3 2
```




```output1
101011
11111
1001
```



## Note

<p>The first test case is described in the problem statement.</p><p>In the second test case all numbers from $1$ to $5$ are beautiful:</p><ul> <li> if $l = 3$ and $r = 3$ we will have a permutation $[1]$ for $m = 1$; </li><li> if $l = 3$ and $r = 4$ we will have a permutation $[1, 2]$ for $m = 2$; </li><li> if $l = 2$ and $r = 4$ we will have a permutation $[3, 1, 2]$ for $m = 3$; </li><li> if $l = 2$ and $r = 5$ we will have a permutation $[3, 1, 2, 4]$ for $m = 4$; </li><li> if $l = 1$ and $r = 5$ we will have a permutation $[5, 3, 1, 2, 4]$ for $m = 5$. </li></ul>
