## Description

<div><p>Alicia has an array, $a_1, a_2, \ldots, a_n$, of non-negative integers. For each $1 \leq i \leq n$, she has found a non-negative integer $x_i = max(0, a_1, \ldots, a_{i-1})$. Note that for $i=1$, $x_i = 0$.</p><p>For example, if Alicia had the array $a = \{0, 1, 2, 0, 3\}$, then $x = \{0, 0, 1, 2, 2\}$.</p><p>Then, she calculated an array, $b_1, b_2, \ldots, b_n$: $b_i = a_i - x_i$.</p><p>For example, if Alicia had the array $a = \{0, 1, 2, 0, 3\}$, $b = \{0-0, 1-0, 2-1, 0-2, 3-2\} = \{0, 1, 1, -2, 1\}$.</p><p>Alicia gives you the values $b_1, b_2, \ldots, b_n$ and asks you to restore the values $a_1, a_2, \ldots, a_n$. Can you help her solve the problem?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($3 \leq n \leq 200\,000$)&nbsp;– the number of elements in Alicia's array.</p><p>The next line contains $n$ integers, $b_1, b_2, \ldots, b_n$ ($-10^9 \leq b_i \leq 10^9$).</p><p>It is guaranteed that for the given array $b$ there is a solution $a_1, a_2, \ldots, a_n$, for all elements of which the following is true: $0 \leq a_i \leq 10^9$.</p></div><div class="output-specification"><p>Print $n$ integers, $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$), such that if you calculate $x$ according to the statement, $b_1$ will be equal to $a_1 - x_1$, $b_2$ will be equal to $a_2 - x_2$, ..., and $b_n$ will be equal to $a_n - x_n$.</p><p>It is guaranteed that there exists at least one solution for the given tests. It can be shown that the solution is unique.</p></div>

## Input

<p>The first line contains one integer $n$ ($3 \leq n \leq 200\,000$)&nbsp;– the number of elements in Alicia's array.</p><p>The next line contains $n$ integers, $b_1, b_2, \ldots, b_n$ ($-10^9 \leq b_i \leq 10^9$).</p><p>It is guaranteed that for the given array $b$ there is a solution $a_1, a_2, \ldots, a_n$, for all elements of which the following is true: $0 \leq a_i \leq 10^9$.</p>

## Output

<p>Print $n$ integers, $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$), such that if you calculate $x$ according to the statement, $b_1$ will be equal to $a_1 - x_1$, $b_2$ will be equal to $a_2 - x_2$, ..., and $b_n$ will be equal to $a_n - x_n$.</p><p>It is guaranteed that there exists at least one solution for the given tests. It can be shown that the solution is unique.</p>





```input1
5
0 1 1 -2 1
```




```input2
3
1000 999999000 -1000000000
```




```input3
5
2 1 2 2 3
```




```output1
0 1 2 0 3
```




```output2
1000 1000000000 0
```




```output3
2 3 5 7 10
```



## Note

<p>The first test was described in the problem statement.</p><p>In the second test, if Alicia had an array $a = \{1000, 1000000000, 0\}$, then $x = \{0, 1000, 1000000000\}$ and $b = \{1000-0, 1000000000-1000, 0-1000000000\} = \{1000, 999999000, -1000000000\}$.</p>
