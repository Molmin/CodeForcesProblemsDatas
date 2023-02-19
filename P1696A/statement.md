## Description

<div><p>NIT, the cleaver, is new in town! Thousands of people line up to orz him. To keep his orzers entertained, NIT decided to let them solve the following problem related to $\operatorname{or} z$. Can you solve this problem too?</p><p>You are given a 1-indexed array of $n$ integers, $a$, and an integer $z$. You can do the following operation any number (possibly zero) of times:</p><ul> <li> Select a positive integer $i$ such that $1\le i\le n$. Then, <span class="tex-font-style-bf">simutaneously</span> set $a_i$ to $(a_i\operatorname{or} z)$ and set $z$ to $(a_i\operatorname{and} z)$. In other words, let $x$ and $y$ respectively be the current values of $a_i$ and $z$. Then set $a_i$ to $(x\operatorname{or}y)$ and set $z$ to $(x\operatorname{and}y)$. </li></ul><p>Here $\operatorname{or}$ and $\operatorname{and}$ denote the <a href="https://en.wikipedia.org/wiki/Bitwise_operation">bitwise operations OR and AND</a> respectively.</p><p>Find the maximum possible value of the maximum value in $a$ after any number (possibly zero) of operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $z$ ($1\le n\le 2000$, $0\le z&lt;2^{30}$).</p><p>The second line of each test case contains $n$ integers $a_1$,$a_2$,$\ldots$,$a_n$ ($0\le a_i&lt;2^{30}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For each test case, print one integer — the answer to the problem.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $z$ ($1\le n\le 2000$, $0\le z&lt;2^{30}$).</p><p>The second line of each test case contains $n$ integers $a_1$,$a_2$,$\ldots$,$a_n$ ($0\le a_i&lt;2^{30}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p>

## Output

<p>For each test case, print one integer — the answer to the problem.</p>





```input1|2,3,6,7,10,11
5
2 3
3 4
5 5
0 2 4 6 8
1 9
10
5 7
7 15 30 29 27
3 39548743
10293834 10284344 13635445
```




```output1
7
13
11
31
48234367
```



## Note

<p>In the first test case of the sample, one optimal sequence of operations is:</p><ul> <li> Do the operation with $i=1$. Now $a_1$ becomes $(3\operatorname{or}3)=3$ and $z$ becomes $(3\operatorname{and}3)=3$. </li><li> Do the operation with $i=2$. Now $a_2$ becomes $(4\operatorname{or}3)=7$ and $z$ becomes $(4\operatorname{and}3)=0$. </li><li> Do the operation with $i=1$. Now $a_1$ becomes $(3\operatorname{or}0)=3$ and $z$ becomes $(3\operatorname{and}0)=0$. </li></ul><p>After these operations, the sequence $a$ becomes $[3,7]$, and the maximum value in it is $7$. We can prove that the maximum value in $a$ can never exceed $7$, so the answer is $7$.</p><p>In the fourth test case of the sample, one optimal sequence of operations is:</p><ul> <li> Do the operation with $i=1$. Now $a_1$ becomes $(7\operatorname{or}7)=7$ and $z$ becomes $(7\operatorname{and}7)=7$. </li><li> Do the operation with $i=3$. Now $a_3$ becomes $(30\operatorname{or}7)=31$ and $z$ becomes $(30\operatorname{and}7)=6$. </li><li> Do the operation with $i=5$. Now $a_5$ becomes $(27\operatorname{or}6)=31$ and $z$ becomes $(27\operatorname{and}6)=2$. </li></ul>
