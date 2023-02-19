## Description

<div><p>You are given an array $a$ of $n$ integers. Count the number of pairs of indices $(i, j)$ such that $i &lt; j$ and $a_j - a_i = j - i$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output the number of pairs of indices $(i, j)$ such that $i &lt; j$ and $a_j - a_i = j - i$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output the number of pairs of indices $(i, j)$ such that $i &lt; j$ and $a_j - a_i = j - i$.</p>





```input1
4
6
3 5 1 4 6 6
3
1 2 3
4
1 3 3 4
6
1 6 3 4 5 6
```




```output1
1
3
3
10
```


