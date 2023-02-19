## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$, which is sorted in non-descending order. You decided to perform the following steps to create array $b_1, b_2, \dots, b_n$: </p><ol> <li> Create an array $d$ consisting of $n$ arbitrary <span class="tex-font-style-bf">non-negative</span> integers. </li><li> Set $b_i = a_i + d_i$ for each $b_i$. </li><li> Sort the array $b$ in non-descending order. </li></ol><p>You are given the resulting array $b$. For each index $i$, calculate what is the minimum and maximum possible value of $d_i$ you can choose in order to get the given array $b$.</p><p>Note that the minimum (maximum) $d_i$-s are <span class="tex-font-style-bf">independent</span> of each other, i.&nbsp;e. they can be obtained from different possible arrays $d$.</p></div><div class="input-specification"><p>The first line contains the single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of arrays $a$, $b$ and $d$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$; $a_i \le a_{i+1}$)&nbsp;— the array $a$ in non-descending order.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$; $b_i \le b_{i+1}$)&nbsp;— the array $b$ in non-descending order.</p><p>Additional constraints on the input: </p><ul> <li> there is at least one way to obtain the array $b$ from the $a$ by choosing an array $d$ consisting of <span class="tex-font-style-bf">non-negative integers</span>; </li><li> the sum of $n$ doesn't exceed $2 \cdot 10^5$. </li></ul></div><div class="output-specification"><p>For each test case, print two lines. In the first line, print $n$ integers $d_1^{min}, d_2^{min}, \dots, d_n^{min}$, where $d_i^{min}$ is the minimum possible value you can add to $a_i$.</p><p>Secondly, print $n$ integers $d_1^{max}, d_2^{max}, \dots, d_n^{max}$, where $d_i^{max}$ is the maximum possible value you can add to $a_i$.</p><p>All $d_i^{min}$ and $d_i^{max}$ values are independent of each other. In other words, for each $i$, $d_i^{min}$ is just the minimum value among all possible values of $d_i$.</p></div>

## Input

<p>The first line contains the single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of arrays $a$, $b$ and $d$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$; $a_i \le a_{i+1}$)&nbsp;— the array $a$ in non-descending order.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$; $b_i \le b_{i+1}$)&nbsp;— the array $b$ in non-descending order.</p><p>Additional constraints on the input: </p><ul> <li> there is at least one way to obtain the array $b$ from the $a$ by choosing an array $d$ consisting of <span class="tex-font-style-bf">non-negative integers</span>; </li><li> the sum of $n$ doesn't exceed $2 \cdot 10^5$. </li></ul>

## Output

<p>For each test case, print two lines. In the first line, print $n$ integers $d_1^{min}, d_2^{min}, \dots, d_n^{min}$, where $d_i^{min}$ is the minimum possible value you can add to $a_i$.</p><p>Secondly, print $n$ integers $d_1^{max}, d_2^{max}, \dots, d_n^{max}$, where $d_i^{max}$ is the maximum possible value you can add to $a_i$.</p><p>All $d_i^{min}$ and $d_i^{max}$ values are independent of each other. In other words, for each $i$, $d_i^{min}$ is just the minimum value among all possible values of $d_i$.</p>





```input1|2,3,4,8,9,10
4
3
2 3 5
7 11 13
1
1000
5000
4
1 2 3 4
1 2 3 4
4
10 20 30 40
22 33 33 55
```




```output1
5 4 2
11 10 8
4000
4000
0 0 0 0
0 0 0 0
12 2 3 15
23 13 3 15
```



## Note

<p>In the first test case, in order to get $d_1^{min} = 5$, we can choose, for example, $d = [5, 10, 6]$. Then $b$ $=$ $[2+5,3+10,5+6]$ $=$ $[7,13,11]$ $=$ $[7,11,13]$.</p><p>For $d_2^{min} = 4$, we can choose $d$ $=$ $[9, 4, 8]$. Then $b$ $=$ $[2+9,3+4,5+8]$ $=$ $[11,7,13]$ $=$ $[7,11,13]$.</p>
