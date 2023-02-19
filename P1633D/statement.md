## Description

<div><p>You have an array of integers $a$ of size $n$. Initially, all elements of the array are equal to $1$. You can perform the following operation: choose two integers $i$ ($1 \le i \le n$) and $x$ ($x &gt; 0$), and then increase the value of $a_i$ by $\left\lfloor\frac{a_i}{x}\right\rfloor$ (i.e. make $a_i = a_i + \left\lfloor\frac{a_i}{x}\right\rfloor$).</p><p>After performing all operations, you will receive $c_i$ coins for all such $i$ that $a_i = b_i$.</p><p>Your task is to determine the maximum number of coins that you can receive by performing no more than $k$ operations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^3; 0 \le k \le 10^6$)&nbsp;— the size of the array and the maximum number of operations, respectively.</p><p>The second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^3$).</p><p>The third line contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le 10^6$).</p><p>The sum of $n$ over all test cases does not exceed $10^3$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the maximum number of coins that you can get by performing no more than $k$ operations.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^3; 0 \le k \le 10^6$)&nbsp;— the size of the array and the maximum number of operations, respectively.</p><p>The second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^3$).</p><p>The third line contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le 10^6$).</p><p>The sum of $n$ over all test cases does not exceed $10^3$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the maximum number of coins that you can get by performing no more than $k$ operations.</p>





```input1|2,3,4,8,9,10
4
4 4
1 7 5 2
2 6 5 2
3 0
3 5 2
5 4 7
5 9
5 2 5 6 3
5 9 1 9 7
6 14
11 4 6 2 8 16
43 45 9 41 15 38
```




```output1
9
0
30
167
```


