## Description

<div><p>RSJ has a sequence $a$ of $n$ integers $a_1,a_2, \ldots, a_n$ and an integer $s$. For each of $a_2,a_3, \ldots, a_{n-1}$, he chose a pair of <span class="tex-font-style-bf">non-negative integers</span> $x_i$ and $y_i$ such that $x_i+y_i=a_i$ and $(x_i-s) \cdot (y_i-s) \geq 0$.</p><p>Now he is interested in the value $$F = a_1 \cdot x_2+y_2 \cdot x_3+y_3 \cdot x_4 + \ldots + y_{n - 2} \cdot x_{n-1}+y_{n-1} \cdot a_n.$$</p><p>Please help him find the minimum possible value $F$ he can get by choosing $x_i$ and $y_i$ optimally. It can be shown that there is always at least one valid way to choose them.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$, $s$ ($3 \le n \le 2 \cdot 10^5$; $0 \le s \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0 \le a_i \le 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum possible value of $F$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$, $s$ ($3 \le n \le 2 \cdot 10^5$; $0 \le s \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0 \le a_i \le 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the minimum possible value of $F$.</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
5 0
2 0 1 3 4
5 1
5 3 4 3 5
7 2
7 6 5 4 3 2 1
5 1
1 2 3 4 5
5 2
1 2 3 4 5
4 0
0 1 1 1
5 5
4 3 5 6 4
4 1
0 2 1 0
3 99999
200000 200000 200000
6 8139
7976 129785 12984 78561 173685 15480
```




```output1
0
18
32
11
14
0
16
0
40000000000
2700826806
```



## Note

<p>In the first test case, $2\cdot 0+0\cdot 1+0\cdot 3+0\cdot 4 = 0$.</p><p>In the second test case, $5\cdot 1+2\cdot 2+2\cdot 2+1\cdot 5 = 18$.</p>
