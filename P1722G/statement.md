## Description

<div><p>Given an integer $n$, find any array $a$ of $n$ <span class="tex-font-style-bf">distinct</span> nonnegative integers less than $2^{31}$ such that the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of the elements on odd indices equals the bitwise XOR of the elements on even indices.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 629$)&nbsp;— the number of test cases.</p><p>Then $t$ lines follow, each containing a single integer $n$ $(3 \leq n \leq 2\cdot10^5)$&nbsp;— the length of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one line containing $n$ distinct integers that satisfy the conditions.</p><p>If there are multiple answers, you can output any of them.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 629$)&nbsp;— the number of test cases.</p><p>Then $t$ lines follow, each containing a single integer $n$ $(3 \leq n \leq 2\cdot10^5)$&nbsp;— the length of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output one line containing $n$ distinct integers that satisfy the conditions.</p><p>If there are multiple answers, you can output any of them.</p>





```input1
7
8
3
4
5
6
7
9
```




```output1
4 2 1 5 0 6 7 3
2 1 3
2 1 3 0
2 0 4 5 3
4 1 2 12 3 8
1 2 3 4 5 6 7
8 2 3 7 4 0 5 6 9
```



## Note

<p>In the first test case the XOR on odd indices is $4 \oplus 1 \oplus 0 \oplus 7 = 2$ and the XOR on even indices is $2 \oplus 5 \oplus 6 \oplus 3= 2$.</p>
