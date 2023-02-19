## Description

<div><p>Tokitsukaze has a permutation $p$ of length $n$. Recall that a permutation $p$ of length $n$ is a sequence $p_1, p_2, \ldots, p_n$ consisting of $n$ distinct integers, each of which from $1$ to $n$ ($1 \leq p_i \leq n$).</p><p>She wants to know how many different indices tuples $[a,b,c,d]$ ($1 \leq a &lt; b &lt; c &lt; d \leq n$) in this permutation satisfy the following two inequalities:</p><center>  $p_a &lt; p_c$ and $p_b &gt; p_d$. </center><p>Note that two tuples $[a_1,b_1,c_1,d_1]$ and $[a_2,b_2,c_2,d_2]$ are considered to be different if $a_1 \ne a_2$ or $b_1 \ne b_2$ or $c_1 \ne c_2$ or $d_1 \ne d_2$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Each test case consists of two lines.</p><p>The first line contains a single integer $n$ ($4 \leq n \leq 5000$)&nbsp;— the length of permutation $p$.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$)&nbsp;— the permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the number of different $[a,b,c,d]$ tuples.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Each test case consists of two lines.</p><p>The first line contains a single integer $n$ ($4 \leq n \leq 5000$)&nbsp;— the length of permutation $p$.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$)&nbsp;— the permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the number of different $[a,b,c,d]$ tuples.</p>





```input1
3
6
5 3 6 1 4 2
4
1 2 3 4
10
5 1 6 2 8 3 4 10 9 7
```




```output1
3
0
28
```



## Note

<p>In the first test case, there are $3$ different $[a,b,c,d]$ tuples.</p><p>$p_1 = 5$, $p_2 = 3$, $p_3 = 6$, $p_4 = 1$, where $p_1 &lt; p_3$ and $p_2 &gt; p_4$ satisfies the inequality, so one of $[a,b,c,d]$ tuples is $[1,2,3,4]$.</p><p>Similarly, other two tuples are $[1,2,3,6]$, $[2,3,5,6]$.</p>
