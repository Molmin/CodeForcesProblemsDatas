## Description

<div><p>You are given $n$ of integers $a_1, a_2, \ldots, a_n$. Process $q$ queries of two types:</p><ul><li> query of the form "<span class="tex-font-style-tt">0 $x_j$</span>": add the value $x_j$ to all even elements of the array $a$,</li><li> query of the form "<span class="tex-font-style-tt">1 $x_j$</span>": add the value $x_j$ to all odd elements of the array $a$.</li></ul><p>Note that when processing the query, we look specifically at the odd/even value of $a_i$, not its index.</p><p>After processing each query, print the sum of the elements of the array $a$.</p><p>Please note that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ $(1 \leq t \leq 10^4$) — the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n$, $q \leq 10^5$) — the length of array $a$ and the number of queries.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — elements of the array $a$.</p><p>The following $q$ lines contain queries as two integers $type_j$ and $x_j$ $(0 \leq type_j \leq 1$, $1 \leq x_j \leq 10^4$).</p><p>It is guaranteed that the sum of values $n$ over all test cases in a test does not exceed $10^5$. Similarly, the sum of values $q$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print $q$ numbers: the sum of the elements of the array $a$ after processing a query.</p></div>

## Input

<p>The first line of the input contains an integer $t$ $(1 \leq t \leq 10^4$) — the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n$, $q \leq 10^5$) — the length of array $a$ and the number of queries.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — elements of the array $a$.</p><p>The following $q$ lines contain queries as two integers $type_j$ and $x_j$ $(0 \leq type_j \leq 1$, $1 \leq x_j \leq 10^4$).</p><p>It is guaranteed that the sum of values $n$ over all test cases in a test does not exceed $10^5$. Similarly, the sum of values $q$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print $q$ numbers: the sum of the elements of the array $a$ after processing a query.</p>





```input1|2,3,4,10,11,12,13,14,15,16,17,18
4
1 1
1
1 1
3 3
1 2 4
0 2
1 3
0 5
6 7
1 3 2 4 10 48
1 6
0 5
0 4
0 5
1 3
0 12
0 1
6 7
1000000000 1000000000 1000000000 11 15 17
0 17
1 10000
1 51
0 92
0 53
1 16
0 1
```




```output1
2
11
14
29
80
100
100
100
118
190
196
3000000094
3000060094
3000060400
3000060952
3000061270
3000061366
3000061366
```



## Note

<p>In the first test case, the array $a = [2]$ after the first query.</p><p>In the third test case, the array $a$ is modified as follows: $[1, 3, 2, 4, 10, 48]$ $\rightarrow$ $[7, 9, 2, 4, 10, 48]$ $\rightarrow$ $[7, 9, 7, 9, 15, 53]$ $\rightarrow$ $[7, 9, 7, 9, 15, 53]$ $\rightarrow$ $[10, 12, 10, 12, 18, 56]$ $\rightarrow$ $[22, 24, 22, 24, 30, 68]$ $\rightarrow$ $[23, 25, 23, 25, 31, 69]$.</p>
