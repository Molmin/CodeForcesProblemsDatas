## Description

<div><p>You have two positive integers $a$ and $b$.</p><p>You can perform two kinds of operations:</p><ul> <li> $a = \lfloor \frac{a}{b} \rfloor$ (replace $a$ with the integer part of the division between $a$ and $b$) </li><li> $b=b+1$ (increase $b$ by $1$) </li></ul><p>Find the minimum number of operations required to make $a=0$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The only line of the description of each test case contains two integers $a$, $b$ ($1 \le a,b \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print a single integer: the minimum number of operations required to make $a=0$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The only line of the description of each test case contains two integers $a$, $b$ ($1 \le a,b \le 10^9$).</p>

## Output

<p>For each test case, print a single integer: the minimum number of operations required to make $a=0$.</p>





```input1
6
9 2
1337 1
1 1
50000000 4
991026972 997
1234 5678
```




```output1
4
9
2
12
3
1
```



## Note

<p>In the first test case, one of the optimal solutions is:</p><ol> <li> Divide $a$ by $b$. After this operation $a = 4$ and $b = 2$. </li><li> Divide $a$ by $b$. After this operation $a = 2$ and $b = 2$. </li><li> Increase $b$. After this operation $a = 2$ and $b = 3$. </li><li> Divide $a$ by $b$. After this operation $a = 0$ and $b = 3$. </li></ol>
