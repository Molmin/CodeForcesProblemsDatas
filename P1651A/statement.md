## Description

<div><p>Consider a playoff tournament where $2^n$ athletes compete. The athletes are numbered from $1$ to $2^n$.</p><p>The tournament is held in $n$ stages. In each stage, the athletes are split into pairs in such a way that each athlete belongs exactly to one pair. In each pair, the athletes compete against each other, and exactly one of them wins. The winner of each pair advances to the next stage, the athlete who was defeated gets eliminated from the tournament.</p><p>The pairs are formed as follows:</p><ul> <li> in the first stage, athlete $1$ competes against athlete $2$; $3$ competes against $4$; $5$ competes against $6$, and so on; </li><li> in the second stage, the winner of the match "$1$–$2$" competes against the winner of the match "$3$–$4$"; the winner of the match "$5$–$6$" competes against the winner of the match "$7$–$8$", and so on; </li><li> the next stages are held according to the same rules. </li></ul><p>When athletes $x$ and $y$ compete, the winner is decided as follows:</p><ul> <li> if $x+y$ is odd, the athlete with the lower index wins (i. e. if $x &lt; y$, then $x$ wins, otherwise $y$ wins); </li><li> if $x+y$ is even, the athlete with the higher index wins. </li></ul><p>The following picture describes the way the tournament with $n = 3$ goes.</p><center> <img class="tex-graphics" src="file://sbeEAtaT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Your task is the following one: given the integer $n$, determine the index of the athlete who wins the tournament.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 30$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 30$).</p></div><div class="output-specification"><p>For each test case, print one integer — the index of the winner of the tournament.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 30$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 30$).</p>

## Output

<p>For each test case, print one integer — the index of the winner of the tournament.</p>





```input1
2
3
1
```




```output1
7
1
```



## Note

<p>The case $n = 3$ is shown in the picture from the statement.</p><p>If $n = 1$, then there's only one match between athletes $1$ and $2$. Since $1 + 2 = 3$ is an odd number, the athlete with the lower index wins. So, the athlete $1$ is the winner.</p>
