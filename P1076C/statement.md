## Description

<div><p>Try guessing the statement from this picture: </p><center> <img class="tex-graphics" src="file://QufsQEE1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a non-negative integer $d$. You have to find two non-negative real numbers $a$ and $b$ such that $a + b = d$ and $a \cdot b = d$.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>Each test case contains one integer $d$ $(0 \le d \le 10^3)$.</p></div><div class="output-specification"><p>For each test print one line.</p><p>If there is an answer for the $i$-th test, print "Y", and then the numbers $a$ and $b$.</p><p>If there is no answer for the $i$-th test, print "N".</p><p>Your answer will be considered correct if $|(a + b) - a \cdot b| \le 10^{-6}$ and $|(a + b) - d| \le 10^{-6}$.</p></div>

## Input

<p>The first line contains $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>Each test case contains one integer $d$ $(0 \le d \le 10^3)$.</p>

## Output

<p>For each test print one line.</p><p>If there is an answer for the $i$-th test, print "Y", and then the numbers $a$ and $b$.</p><p>If there is no answer for the $i$-th test, print "N".</p><p>Your answer will be considered correct if $|(a + b) - a \cdot b| \le 10^{-6}$ and $|(a + b) - d| \le 10^{-6}$.</p>





```input1
7
69
0
1
4
5
999
1000
```




```output1
Y 67.985071301 1.014928699
Y 0.000000000 0.000000000
N
Y 2.000000000 2.000000000
Y 3.618033989 1.381966011
Y 997.998996990 1.001003010
Y 998.998997995 1.001002005
```


