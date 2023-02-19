## Description

<div><p>Stanley defines the beauty of an array $a$ of length $n$, which contains <span class="tex-font-style-bf">non-negative integers</span>, as follows: $$\sum\limits_{i = 1}^{n} \left \lfloor \frac{a_{i}}{k} \right \rfloor,$$ which means that we divide each element by $k$, round it down, and sum up the resulting values.</p><p>Stanley told Sam the integer $k$ and asked him to find an array $a$ of $n$ non-negative integers, such that the beauty is equal to $b$ and the sum of elements is equal to $s$. Help Sam&nbsp;— find any of the arrays satisfying the conditions above.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains integers $n$, $k$, $b$, $s$ ($1 \leq n \leq 10^{5}$, $1 \leq k \leq 10^{9}$, $0 \leq b \leq 10^{9}$, $0 \leq s \leq 10^{18}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print $-1$ if such array $a$ does not exist. Otherwise print $n$ non-negative integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_{i} \leq 10^{18}$)&nbsp;— the answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains integers $n$, $k$, $b$, $s$ ($1 \leq n \leq 10^{5}$, $1 \leq k \leq 10^{9}$, $0 \leq b \leq 10^{9}$, $0 \leq s \leq 10^{18}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print $-1$ if such array $a$ does not exist. Otherwise print $n$ non-negative integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_{i} \leq 10^{18}$)&nbsp;— the answer.</p>





```input1|2,4,6,8
8
1 6 3 100
3 6 3 12
3 6 3 19
5 4 7 38
5 4 7 80
99978 1000000000 100000000 1000000000000000000
1 1 0 0
4 1000000000 1000000000 1000000000000000000
```




```output1
-1
-1
0 0 19
0 3 3 3 29
-1
-1
0
0 0 0 1000000000000000000
```



## Note

<p>In the first, the second, the fifth and the sixth test cases of the example it is possible to show that such array does not exist.</p><p>In the third testcase of the example $a = [0, 0, 19]$. The sum of elements in it is equal to 19, the beauty of it is equal to $\left ( \left \lfloor \frac{0}{6} \right \rfloor + \left \lfloor \frac{0}{6} \right \rfloor + \left \lfloor \frac{19}{6} \right \rfloor \right ) = (0 + 0 + 3) = 3$.</p><p>In the fourth testcase of the example $a = [0, 3, 3, 3, 29]$. The sum of elements in it is equal to $38$, the beauty of it is equal to $(0 + 0 + 0 + 0 + 7) = 7$.</p>
