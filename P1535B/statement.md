## Description

<div><p>You are given an array $a$ consisting of $n$ integers.</p><p>Let's call a pair of indices $i$, $j$ <span class="tex-font-style-bf">good</span> if $1 \le i &lt; j \le n$ and $\gcd(a_i, 2a_j) &gt; 1$ (where $\gcd(x, y)$ is the greatest common divisor of $x$ and $y$).</p><p>Find the maximum number of <span class="tex-font-style-bf">good</span> index pairs if you can reorder the array $a$ in an arbitrary way.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of the test case contains a single integer $n$ ($2 \le n \le 2000$)&nbsp;— the number of elements in the array.</p><p>The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the maximum number of <span class="tex-font-style-bf">good</span> index pairs if you can reorder the array $a$ in an arbitrary way.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of the test case contains a single integer $n$ ($2 \le n \le 2000$)&nbsp;— the number of elements in the array.</p><p>The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the maximum number of <span class="tex-font-style-bf">good</span> index pairs if you can reorder the array $a$ in an arbitrary way.</p>





```input1
3
4
3 6 5 3
2
1 7
5
1 4 2 4 1
```




```output1
4
0
9
```



## Note

<p>In the first example, the array elements can be rearranged as follows: $[6, 3, 5, 3]$.</p><p>In the third example, the array elements can be rearranged as follows: $[4, 4, 2, 1, 1]$.</p>
