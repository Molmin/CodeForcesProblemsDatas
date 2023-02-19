## Description

<div><p>For an array $c$ of nonnegative integers, $MEX(c)$ denotes the smallest nonnegative integer that doesn't appear in it. For example, $MEX([0, 1, 3]) = 2$, $MEX([42]) = 0$.</p><p>You are given integers $n, k$, and an array $[b_1, b_2, \ldots, b_n]$.</p><p>Find the number of arrays $[a_1, a_2, \ldots, a_n]$, for which the following conditions hold:</p><ul><li><p>$0 \le a_i \le n$ for each $i$ for each $i$ from $1$ to $n$.</p></li><li><p>$|MEX([a_1, a_2, \ldots, a_i]) - b_i| \le k$ for each $i$ from $1$ to $n$.</p></li></ul><p>As this number can be very big, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n, k$ ($1 \le n \le 2000$, $0 \le k \le 50$).</p><p>The second line of the input contains $n$ integers $b_1, b_2, \ldots, b_n$ ($-k \le b_i \le n+k$)&nbsp;— elements of the array $b$.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of arrays which satisfy the conditions from the statement, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of the input contains two integers $n, k$ ($1 \le n \le 2000$, $0 \le k \le 50$).</p><p>The second line of the input contains $n$ integers $b_1, b_2, \ldots, b_n$ ($-k \le b_i \le n+k$)&nbsp;— elements of the array $b$.</p>

## Output

<p>Output a single integer&nbsp;— the number of arrays which satisfy the conditions from the statement, modulo $998\,244\,353$.</p>





```input1
4 0
0 0 0 0
```




```input2
4 1
0 0 0 0
```




```input3
4 1
0 0 1 1
```




```input4
5 2
0 0 2 2 0
```




```input5
3 2
-2 0 4
```




```output1
256
```




```output2
431
```




```output3
509
```




```output4
6546
```




```output5
11
```


