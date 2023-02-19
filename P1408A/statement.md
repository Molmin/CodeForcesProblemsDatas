## Description

<div><p>You are given three sequences: $a_1, a_2, \ldots, a_n$; $b_1, b_2, \ldots, b_n$; $c_1, c_2, \ldots, c_n$.</p><p>For each $i$, $a_i \neq b_i$, $a_i \neq c_i$, $b_i \neq c_i$.</p><p>Find a sequence $p_1, p_2, \ldots, p_n$, that satisfy the following conditions:</p><ul><li> $p_i \in \{a_i, b_i, c_i\}$</li><li> $p_i \neq p_{(i \mod n) + 1}$.</li></ul><p>In other words, for each element, you need to choose one of the three possible values, such that no two adjacent elements (where we consider elements $i,i+1$ adjacent for $i&lt;n$ and also elements $1$ and $n$) will have equal value.</p><p>It can be proved that in the given constraints solution always exists. You don't need to minimize/maximize anything, you need to find any proper sequence.</p></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \leq t \leq 100$): the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($3 \leq n \leq 100$): the number of elements in the given sequences.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$).</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 100$).</p><p>The fourth line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq 100$).</p><p>It is guaranteed that $a_i \neq b_i$, $a_i \neq c_i$, $b_i \neq c_i$ for all $i$.</p></div><div class="output-specification"><p>For each test case, print $n$ integers: $p_1, p_2, \ldots, p_n$ ($p_i \in \{a_i, b_i, c_i\}$, $p_i \neq p_{i \mod n + 1}$).</p><p>If there are several solutions, you can print any.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \leq t \leq 100$): the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($3 \leq n \leq 100$): the number of elements in the given sequences.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$).</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 100$).</p><p>The fourth line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq 100$).</p><p>It is guaranteed that $a_i \neq b_i$, $a_i \neq c_i$, $b_i \neq c_i$ for all $i$.</p>

## Output

<p>For each test case, print $n$ integers: $p_1, p_2, \ldots, p_n$ ($p_i \in \{a_i, b_i, c_i\}$, $p_i \neq p_{i \mod n + 1}$).</p><p>If there are several solutions, you can print any.</p>





```input1
5
3
1 1 1
2 2 2
3 3 3
4
1 2 1 2
2 1 2 1
3 4 3 4
7
1 3 3 1 1 1 1
2 4 4 3 2 2 4
4 2 2 2 4 4 2
3
1 2 1
2 3 3
3 1 2
10
1 1 1 2 2 2 3 3 3 1
2 2 2 3 3 3 1 1 1 2
3 3 3 1 1 1 2 2 2 3
```




```output1
1 2 3
1 2 1 2
1 3 4 3 2 4 2
1 3 2
1 2 3 1 2 3 1 2 3 2
```



## Note

<p>In the first test case $p = [1, 2, 3]$.</p><p>It is a correct answer, because:</p><ul> <li> $p_1 = 1 = a_1$, $p_2 = 2 = b_2$, $p_3 = 3 = c_3$ </li><li> $p_1 \neq p_2 $, $p_2 \neq p_3 $, $p_3 \neq p_1$ </li></ul><p>All possible correct answers to this test case are: $[1, 2, 3]$, $[1, 3, 2]$, $[2, 1, 3]$, $[2, 3, 1]$, $[3, 1, 2]$, $[3, 2, 1]$.</p><p>In the second test case $p = [1, 2, 1, 2]$.</p><p>In this sequence $p_1 = a_1$, $p_2 = a_2$, $p_3 = a_3$, $p_4 = a_4$. Also we can see, that no two adjacent elements of the sequence are equal.</p><p>In the third test case $p = [1, 3, 4, 3, 2, 4, 2]$.</p><p>In this sequence $p_1 = a_1$, $p_2 = a_2$, $p_3 = b_3$, $p_4 = b_4$, $p_5 = b_5$, $p_6 = c_6$, $p_7 = c_7$. Also we can see, that no two adjacent elements of the sequence are equal.</p>
