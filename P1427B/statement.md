## Description

<div><p>You like playing chess tournaments online.</p><p>In your last tournament you played $n$ games. For the sake of this problem, each chess game is either won or lost (no draws). When you lose a game you get $0$ points. When you win you get $1$ or $2$ points: if you have won also the previous game you get $2$ points, otherwise you get $1$ point. If you win the very first game of the tournament you get $1$ point (since there is not a "previous game").</p><p>The outcomes of the $n$ games are represented by a string $s$ of length $n$: the $i$-th character of $s$ is <span class="tex-font-style-tt">W</span> if you have won the $i$-th game, while it is <span class="tex-font-style-tt">L</span> if you have lost the $i$-th game.</p><p>After the tournament, you notice a bug on the website that allows you to change the outcome of <span class="tex-font-style-bf">at most</span> $k$ of your games (meaning that at most $k$ times you can change some symbol <span class="tex-font-style-tt">L</span> to <span class="tex-font-style-tt">W</span>, or <span class="tex-font-style-tt">W</span> to <span class="tex-font-style-tt">L</span>). Since your only goal is to improve your chess rating, you decide to cheat and use the bug.</p><p>Compute the maximum score you can get by cheating in the optimal way.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t \le 20,000$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each testcase contains two integers $n, k$ ($1\le n\le 100,000$, $0\le k\le n$) – the number of games played and the number of outcomes that you can change.</p><p>The second line contains a string $s$ of length $n$ containing only the characters <span class="tex-font-style-tt">W</span> and <span class="tex-font-style-tt">L</span>. If you have won the $i$-th game then $s_i=\,$<span class="tex-font-style-tt">W</span>, if you have lost the $i$-th game then $s_i=\,$<span class="tex-font-style-tt">L</span>.</p><p>It is guaranteed that the sum of $n$ over all testcases does not exceed $200,000$.</p></div><div class="output-specification"><p>For each testcase, print a single integer – the maximum score you can get by cheating in the optimal way.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t \le 20,000$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each testcase contains two integers $n, k$ ($1\le n\le 100,000$, $0\le k\le n$) – the number of games played and the number of outcomes that you can change.</p><p>The second line contains a string $s$ of length $n$ containing only the characters <span class="tex-font-style-tt">W</span> and <span class="tex-font-style-tt">L</span>. If you have won the $i$-th game then $s_i=\,$<span class="tex-font-style-tt">W</span>, if you have lost the $i$-th game then $s_i=\,$<span class="tex-font-style-tt">L</span>.</p><p>It is guaranteed that the sum of $n$ over all testcases does not exceed $200,000$.</p>

## Output

<p>For each testcase, print a single integer – the maximum score you can get by cheating in the optimal way.</p>





```input1
8
5 2
WLWLL
6 5
LLLWWL
7 1
LWLWLWL
15 5
WWWLLLWWWLLLWWW
40 7
LLWLWLWWWLWLLWLWWWLWLLWLLWLLLLWLLWWWLWWL
1 0
L
1 1
L
6 1
WLLWLW
```




```output1
7
11
6
26
46
0
1
6
```



## Note

<p><span class="tex-font-style-bf">Explanation of the first testcase.</span> Before changing any outcome, the score is $2$. Indeed, you won the first game, so you got $1$ point, and you won also the third, so you got another $1$ point (and not $2$ because you lost the second game).</p><p>An optimal way to cheat is to change the outcomes of the second and fourth game. Doing so, you end up winning the first four games (the string of the outcomes becomes <span class="tex-font-style-tt">WWWWL</span>). Hence, the new score is $7=1+2+2+2$: $1$ point for the first game and $2$ points for the second, third and fourth game.</p><p><span class="tex-font-style-bf">Explanation of the second testcase.</span> Before changing any outcome, the score is $3$. Indeed, you won the fourth game, so you got $1$ point, and you won also the fifth game, so you got $2$ more points (since you won also the previous game).</p><p>An optimal way to cheat is to change the outcomes of the first, second, third and sixth game. Doing so, you end up winning all games (the string of the outcomes becomes <span class="tex-font-style-tt">WWWWWW</span>). Hence, the new score is $11 = 1+2+2+2+2+2$: $1$ point for the first game and $2$ points for all the other games.</p>
