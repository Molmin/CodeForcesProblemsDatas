## Description

<div><p>You are given an array of $n$ positive integers $a_1, a_2, \ldots, a_n$. Your task is to calculate the number of arrays of $n$ positive integers $b_1, b_2, \ldots, b_n$ such that: </p><ul> <li> $1 \le b_i \le a_i$ for every $i$ ($1 \le i \le n$), and </li><li> $b_i \neq b_{i+1}$ for every $i$ ($1 \le i \le n - 1$). </li></ul><p>The number of such arrays can be very large, so print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Print the answer modulo $998\,244\,353$ in a single line.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>Print the answer modulo $998\,244\,353$ in a single line.</p>





```input1
3
2 2 2
```




```input2
2
2 3
```




```input3
3
1 1 1
```




```output1
2
```




```output2
4
```




```output3
0
```



## Note

<p>In the first test case possible arrays are $[1, 2, 1]$ and $[2, 1, 2]$.</p><p>In the second test case possible arrays are $[1, 2]$, $[1, 3]$, $[2, 1]$ and $[2, 3]$.</p>
