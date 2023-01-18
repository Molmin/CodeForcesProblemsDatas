## Description

<div><p>Polycarp, Arkady's friend, prepares to the programming competition and decides to write a contest. The contest consists of $n$ problems and lasts for $T$ minutes. Each of the problems is defined by two positive integers $a_i$ and $p_i$&nbsp;— its difficulty and the score awarded by its solution.</p><p>Polycarp's experience suggests that his skill level is defined with positive real value $s$, and initially $s=1.0$. To solve the $i$-th problem Polycarp needs $a_i/s$ minutes.</p><p>Polycarp loves to watch series, and before solving each of the problems he will definitely watch one episode. After Polycarp watches an episode, his skill decreases by $10\%$, that is skill level $s$ decreases to $0.9s$. Each episode takes exactly $10$ minutes to watch. When Polycarp decides to solve some problem, he firstly has to watch one episode, and only then he starts solving the problem without breaks for $a_i/s$ minutes, where $s$ is his current skill level. In calculation of $a_i/s$ no rounding is performed, only division of integer value $a_i$ by real value $s$ happens.</p><p>Also, Polycarp can train for some time. If he trains for $t$ minutes, he increases his skill by $C \cdot t$, where $C$ is some given positive real constant. Polycarp can train only before solving any problem (and before watching series). Duration of the training can be arbitrary real value.</p><p>Polycarp is interested: what is the largest score he can get in the contest? It is allowed to solve problems in any order, while training is only allowed <span class="tex-font-style-bf">before solving the first problem</span>.</p></div><div class="input-specification"><p>The first line contains one integer $tc$ ($1 \le tc \le 20$)&nbsp;— the number of test cases. Then $tc$ test cases follow.</p><p>The first line of each test contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the number of problems in the contest.</p><p>The second line of the test contains two real values $C, T$ ($0 &lt; C &lt; 10$, $0 \le T \le 2 \cdot 10^5$), where $C$ defines the efficiency of the training and $T$ is the duration of the contest in minutes. Value $C, T$ are given exactly with three digits after the decimal point.</p><p>Each of the next $n$ lines of the test contain characteristics of the corresponding problem: two integers $a_i, p_i$ ($1 \le a_i \le 10^4$, $1 \le p_i \le 10$)&nbsp;— the difficulty and the score of the problem.</p><p>It is guaranteed that the value of $T$ is such that changing it by the $0.001$ in any direction will not change the test answer.</p><p>Please note that in <span class="tex-font-style-bf">hacks</span> you can only use $tc = 1$.</p></div><div class="output-specification"><p>Print $tc$ integers&nbsp;— the maximum possible score in each test case.</p></div>

## Input

<p>The first line contains one integer $tc$ ($1 \le tc \le 20$)&nbsp;— the number of test cases. Then $tc$ test cases follow.</p><p>The first line of each test contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the number of problems in the contest.</p><p>The second line of the test contains two real values $C, T$ ($0 &lt; C &lt; 10$, $0 \le T \le 2 \cdot 10^5$), where $C$ defines the efficiency of the training and $T$ is the duration of the contest in minutes. Value $C, T$ are given exactly with three digits after the decimal point.</p><p>Each of the next $n$ lines of the test contain characteristics of the corresponding problem: two integers $a_i, p_i$ ($1 \le a_i \le 10^4$, $1 \le p_i \le 10$)&nbsp;— the difficulty and the score of the problem.</p><p>It is guaranteed that the value of $T$ is such that changing it by the $0.001$ in any direction will not change the test answer.</p><p>Please note that in <span class="tex-font-style-bf">hacks</span> you can only use $tc = 1$.</p>

## Output

<p>Print $tc$ integers&nbsp;— the maximum possible score in each test case.</p>





```input1
2
4
1.000 31.000
12 3
20 6
30 1
5 1
3
1.000 30.000
1 10
10 10
20 8

```




```output1
7
20

```



## Note

<p>In the first example, Polycarp can get score of $7$ as follows:</p><ol> <li> Firstly he trains for $4$ minutes, increasing $s$ to the value of $5$; </li><li> Then he decides to solve $4$-th problem: he watches one episode in $10$ minutes, his skill level decreases to $s=5*0.9=4.5$ and then he solves the problem in $5/s=5/4.5$, which is roughly $1.111$ minutes; </li><li> Finally, he decides to solve $2$-nd problem: he watches one episode in $10$ minutes, his skill level decreases to $s=4.5*0.9=4.05$ and then he solves the problem in $20/s=20/4.05$, which is roughly $4.938$ minutes. </li></ol><p>This way, Polycarp uses roughly $4+10+1.111+10+4.938=30.049$ minutes, to get score of $7$ points. It is not possible to achieve larger score in $31$ minutes.</p><p>In the second example, Polycarp can get $20$ points as follows:</p><ol> <li> Firstly he trains for $4$ minutes, increasing $s$ to the value of $5$; </li><li> Then he decides to solve $1$-st problem: he watches one episode in $10$ minutes, his skill decreases to $s=5*0.9=4.5$ and then he solves problem in $1/s=1/4.5$, which is roughly $0.222$ minutes. </li><li> Finally, he decides to solve $2$-nd problem: he watches one episode in $10$ minutes, his skill decreases to $s=4.5*0.9=4.05$ and then he solves the problem in $10/s=10/4.05$, which is roughly $2.469$ minutes. </li></ol><p>This way, Polycarp gets score of $20$ in $4+10+0.222+10+2.469=26.691$ minutes. It is not possible to achieve larger score in $30$ minutes.</p>
