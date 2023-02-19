## Description

<div><p>You are given two arrays $a$ and $b$, consisting of $n$ integers each.</p><p>Let's define a function $f(a, b)$ as follows: </p><ul> <li> let's define an array $c$ of size $n$, where $c_i = a_i \oplus b_i$ ($\oplus$ denotes bitwise XOR); </li><li> the value of the function is $c_1 \mathbin{\&amp;} c_2 \mathbin{\&amp;} \cdots \mathbin{\&amp;} c_n$ (i.e. bitwise AND of the entire array $c$). </li></ul><p>Find the maximum value of the function $f(a, b)$ if you can reorder the array $b$ in an arbitrary way (leaving the initial order is also an option).</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the size of arrays $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; 2^{30}$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i &lt; 2^{30}$).</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the maximum value of the function $f(a, b)$ if you can reorder the array $b$ in an arbitrary way.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the size of arrays $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; 2^{30}$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i &lt; 2^{30}$).</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print one integer&nbsp;— the maximum value of the function $f(a, b)$ if you can reorder the array $b$ in an arbitrary way.</p>





```input1|2,3,4,8,9,10
3
5
1 0 0 3 3
2 3 2 1 0
3
1 1 1
0 0 3
8
0 1 2 3 4 5 6 7
7 6 5 4 3 2 1 0
```




```output1
2
0
7
```


