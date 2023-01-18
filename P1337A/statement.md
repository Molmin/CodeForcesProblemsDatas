## Description

<div><p>Ichihime is the current priestess of the Mahjong Soul Temple. She claims to be human, despite her cat ears.</p><p>These days the temple is holding a math contest. Usually, Ichihime lacks interest in these things, but this time the prize for the winner is her favorite — cookies. Ichihime decides to attend the contest. Now she is solving the following problem.</p><center><img class="tex-graphics" src="file://aqJ6UYjS.png" style="max-width: 100.0%;max-height: 100.0%;"></center>&nbsp;<p>You are given four positive integers $a$, $b$, $c$, $d$, such that $a \leq b \leq c \leq d$. </p><p>Your task is to find three integers $x$, $y$, $z$, satisfying the following conditions:</p><ul><li> $a \leq x \leq b$.</li><li> $b \leq y \leq c$.</li><li> $c \leq z \leq d$.</li><li> There exists a triangle with a positive non-zero area and the lengths of its three sides are $x$, $y$, and $z$.</li></ul><p>Ichihime desires to get the cookie, but the problem seems too hard for her. Can you help her?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$) &nbsp;— the number of test cases.</p><p>The next $t$ lines describe test cases. Each test case is given as four space-separated integers $a$, $b$, $c$, $d$ ($1 \leq a \leq b \leq c \leq d \leq 10^9$).</p></div><div class="output-specification"><p>For each test case, print three integers $x$, $y$, $z$ &nbsp;— the integers you found satisfying the conditions given in the statement.</p><p>It is guaranteed that the answer always exists. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$) &nbsp;— the number of test cases.</p><p>The next $t$ lines describe test cases. Each test case is given as four space-separated integers $a$, $b$, $c$, $d$ ($1 \leq a \leq b \leq c \leq d \leq 10^9$).</p>

## Output

<p>For each test case, print three integers $x$, $y$, $z$ &nbsp;— the integers you found satisfying the conditions given in the statement.</p><p>It is guaranteed that the answer always exists. If there are multiple answers, print any.</p>





```input1
4
1 3 5 7
1 5 5 7
100000 200000 300000 400000
1 1 977539810 977539810
```




```output1
3 4 5
5 5 5
182690 214748 300999
1 977539810 977539810
```



## Note

<p>One of the possible solutions to the first test case:</p><p><img class="tex-graphics" src="file://SI0spogl.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>One of the possible solutions to the second test case:</p><p><img class="tex-graphics" src="file://bFl7J0wO.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
