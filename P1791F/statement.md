## Description

<div><p>Given an array $a_1, a_2, \dots, a_n$, you need to handle a total of $q$ updates and queries of two types:</p><ul> <li> $1$&nbsp;$l$&nbsp;$r$&nbsp;— for each index $i$ with $l \leq i \leq r$, update the value of $a_i$ to the sum of the digits of $a_i$. </li><li> $2$&nbsp;$x$&nbsp;— output $a_x$. </li></ul></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the size of the array and the number of queries, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>The next $q$ lines of each test case are of two forms:</p><ul> <li> $1$&nbsp;$l$&nbsp;$r$ ($1 \leq l \leq r \leq n$)&nbsp;— it means, for each index $i$ with $l \leq i \leq r$, you should update the value of $a_i$ to the sum of its digits. </li><li> $2$&nbsp;$x$ ($1 \leq x \leq n$)&nbsp;— it means you should output $a_x$. </li></ul><p>There is at least one query of the second type.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p><p>The sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the answers of queries of the second type, in the order they are given.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the size of the array and the number of queries, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>The next $q$ lines of each test case are of two forms:</p><ul> <li> $1$&nbsp;$l$&nbsp;$r$ ($1 \leq l \leq r \leq n$)&nbsp;— it means, for each index $i$ with $l \leq i \leq r$, you should update the value of $a_i$ to the sum of its digits. </li><li> $2$&nbsp;$x$ ($1 \leq x \leq n$)&nbsp;— it means you should output $a_x$. </li></ul><p>There is at least one query of the second type.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p><p>The sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the answers of queries of the second type, in the order they are given.</p>





```input1|2,3,4,5,6,7,8,9,10,11,17,18,19
3
5 8
1 420 69 1434 2023
1 2 3
2 2
2 3
2 4
1 2 5
2 1
2 3
2 5
2 3
9999 1000
1 1 2
2 1
2 2
1 1
1
2 1
```




```output1
6
15
1434
1
6
7
36
1
1
```



## Note

<p>In the first test case, the following process occurs: </p><ul> <li> Initially, $a = [1, 420, 69, 1434, 2023]$. </li><li> The operation is performed for $l=2$, $r=3$, yielding $[1, \color{red}{6}, \color{red}{15}, 1434, 2023]$. </li><li> We are queried for $x=2$, $x=3$, and $x=4$, and output $6$, $15$, and $1434$. </li><li> The operation is performed for $l=2$, $r=5$, yielding $[1, \color{red}{6}, \color{red}{6}, \color{red}{12}, \color{red}{7}]$. </li><li> We are queried for $x=1$, $x=3$, and $x=5$, and output $1$, $6$, and $7$. </li></ul>
