## Description

<div><p>You are given a digital clock with $n$ digits. Each digit shows an integer from $0$ to $9$, so the whole clock shows an integer from $0$ to $10^n-1$. The clock will show leading zeroes if the number is smaller than $10^{n-1}$.</p><p>You want the clock to show $0$ with as few operations as possible. In an operation, you can do one of the following: </p><ul> <li> decrease the number on the clock by $1$, or </li><li> swap two digits (you can choose which digits to swap, and they don't have to be adjacent). </li></ul><p>Your task is to determine the minimum number of operations needed to make the clock show $0$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$).</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) — number of digits on the clock.</p><p>The second line of each test case contains a string of $n$ digits $s_1, s_2, \ldots, s_n$ ($0 \le s_1, s_2, \ldots, s_n \le 9$) — the number on the clock.</p><p>Note: If the number is smaller than $10^{n-1}$ the clock will show leading zeroes.</p></div><div class="output-specification"><p>For each test case, print one integer: the minimum number of operations needed to make the clock show $0$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$).</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) — number of digits on the clock.</p><p>The second line of each test case contains a string of $n$ digits $s_1, s_2, \ldots, s_n$ ($0 \le s_1, s_2, \ldots, s_n \le 9$) — the number on the clock.</p><p>Note: If the number is smaller than $10^{n-1}$ the clock will show leading zeroes.</p>

## Output

<p>For each test case, print one integer: the minimum number of operations needed to make the clock show $0$.</p>





```input1
7
3
007
4
1000
5
00000
3
103
4
2020
9
123456789
30
001678294039710047203946100020
```




```output1
7
2
0
5
6
53
115
```



## Note

<p>In the first example, it's optimal to just decrease the number $7$ times.</p><p>In the second example, we can first swap the first and last position and then decrease the number by $1$.</p><p>In the third example, the clock already shows $0$, so we don't have to perform any operations.</p>
