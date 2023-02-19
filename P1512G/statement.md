## Description

<div><p>Let us denote by $d(n)$ the sum of all divisors of the number $n$, i.e. $d(n) = \sum\limits_{k | n} k$.</p><p>For example, $d(1) = 1$, $d(4) = 1+2+4=7$, $d(6) = 1+2+3+6=12$.</p><p>For a given number $c$, find the minimum $n$ such that $d(n) = c$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case is characterized by one integer $c$ ($1 \le c \le 10^7$).</p></div><div class="output-specification"><p>For each test case, output: </p><ul> <li> "<span class="tex-font-style-tt">-1</span>" if there is no such $n$ that $d(n) = c$; </li><li> $n$, otherwise. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case is characterized by one integer $c$ ($1 \le c \le 10^7$).</p>

## Output

<p>For each test case, output: </p><ul> <li> "<span class="tex-font-style-tt">-1</span>" if there is no such $n$ that $d(n) = c$; </li><li> $n$, otherwise. </li></ul>





```input1
12
1
2
3
4
5
6
7
8
9
10
39
691
```




```output1
1
-1
2
3
-1
5
4
7
-1
-1
18
-1
```


