## Description

<div><p>A frog is currently at the point $0$ on a coordinate axis $Ox$. It jumps by the following algorithm: the first jump is $a$ units to the right, the second jump is $b$ units to the left, the third jump is $a$ units to the right, the fourth jump is $b$ units to the left, and so on.</p><p>Formally: </p><ul> <li> if the frog has jumped an even number of times (before the current jump), it jumps from its current position $x$ to position $x+a$; </li><li> otherwise it jumps from its current position $x$ to position $x-b$. </li></ul><p>Your task is to calculate the position of the frog after $k$ jumps.</p><p>But... One more thing. You are watching $t$ different frogs so you have to answer $t$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) — the number of queries.</p><p>Each of the next $t$ lines contain queries (one query per line).</p><p>The query is described as three space-separated integers $a, b, k$ ($1 \le a, b, k \le 10^9$) — the lengths of two types of jumps and the number of jumps, respectively.</p></div><div class="output-specification"><p>Print $t$ integers. The $i$-th integer should be the answer for the $i$-th query.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) — the number of queries.</p><p>Each of the next $t$ lines contain queries (one query per line).</p><p>The query is described as three space-separated integers $a, b, k$ ($1 \le a, b, k \le 10^9$) — the lengths of two types of jumps and the number of jumps, respectively.</p>

## Output

<p>Print $t$ integers. The $i$-th integer should be the answer for the $i$-th query.</p>





```input1
6
5 2 3
100 1 4
1 10 5
1000000000 1 6
1 1 1000000000
1 1 999999999
```




```output1
8
198
-17
2999999997
0
1
```



## Note

<p>In the first query frog jumps $5$ to the right, $2$ to the left and $5$ to the right so the answer is $5 - 2 + 5 = 8$.</p><p>In the second query frog jumps $100$ to the right, $1$ to the left, $100$ to the right and $1$ to the left so the answer is $100 - 1 + 100 - 1 = 198$.</p><p>In the third query the answer is $1 - 10 + 1 - 10 + 1 = -17$.</p><p>In the fourth query the answer is $10^9 - 1 + 10^9 - 1 + 10^9 - 1 = 2999999997$.</p><p>In the fifth query all frog's jumps are neutralized by each other so the answer is $0$.</p><p>The sixth query is the same as the fifth but without the last jump so the answer is $1$.</p>
