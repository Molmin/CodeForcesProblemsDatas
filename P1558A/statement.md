## Description

<div><p>Alice and Borys are playing tennis.</p><p>A tennis match consists of <span class="tex-font-style-it">games</span>. In each game, one of the players is <span class="tex-font-style-it">serving</span> and the other one is <span class="tex-font-style-it">receiving</span>.</p><p>Players serve in turns: after a game where Alice is serving follows a game where Borys is serving, and vice versa.</p><p>Each game ends with a victory of one of the players. If a game is won by the serving player, it's said that this player <span class="tex-font-style-it">holds serve</span>. If a game is won by the receiving player, it's said that this player <span class="tex-font-style-it">breaks serve</span>.</p><p>It is known that Alice won $a$ games and Borys won $b$ games during the match. It is unknown who served first and who won which games.</p><p>Find all values of $k$ such that exactly $k$ breaks could happen during the match between Alice and Borys in total.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Description of the test cases follows.</p><p>Each of the next $t$ lines describes one test case and contains two integers $a$ and $b$ ($0 \le a, b \le 10^5$; $a + b &gt; 0$)&nbsp;— the number of games won by Alice and Borys, respectively.</p><p>It is guaranteed that the sum of $a + b$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print two lines.</p><p>In the first line, print a single integer $m$&nbsp;($1 \le m \le a + b + 1$)&nbsp;— the number of values of $k$ such that exactly $k$ breaks could happen during the match.</p><p>In the second line, print $m$ distinct integers $k_1, k_2, \ldots, k_m$ ($0 \le k_1 &lt; k_2 &lt; \ldots &lt; k_m \le a + b$)&nbsp;— the sought values of $k$ <span class="tex-font-style-bf">in increasing order</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Description of the test cases follows.</p><p>Each of the next $t$ lines describes one test case and contains two integers $a$ and $b$ ($0 \le a, b \le 10^5$; $a + b &gt; 0$)&nbsp;— the number of games won by Alice and Borys, respectively.</p><p>It is guaranteed that the sum of $a + b$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print two lines.</p><p>In the first line, print a single integer $m$&nbsp;($1 \le m \le a + b + 1$)&nbsp;— the number of values of $k$ such that exactly $k$ breaks could happen during the match.</p><p>In the second line, print $m$ distinct integers $k_1, k_2, \ldots, k_m$ ($0 \le k_1 &lt; k_2 &lt; \ldots &lt; k_m \le a + b$)&nbsp;— the sought values of $k$ <span class="tex-font-style-bf">in increasing order</span>.</p>





```input1
3
2 1
1 1
0 5
```




```output1
4
0 1 2 3
2
0 2
2
2 3
```



## Note

<p>In the first test case, any number of breaks between $0$ and $3$ could happen during the match: </p><ul> <li> Alice holds serve, Borys holds serve, Alice holds serve: $0$ breaks; </li><li> Borys holds serve, Alice holds serve, Alice breaks serve: $1$ break; </li><li> Borys breaks serve, Alice breaks serve, Alice holds serve: $2$ breaks; </li><li> Alice breaks serve, Borys breaks serve, Alice breaks serve: $3$ breaks. </li></ul><p>In the second test case, the players could either both hold serves ($0$ breaks) or both break serves ($2$ breaks).</p><p>In the third test case, either $2$ or $3$ breaks could happen: </p><ul> <li> Borys holds serve, Borys breaks serve, Borys holds serve, Borys breaks serve, Borys holds serve: $2$ breaks; </li><li> Borys breaks serve, Borys holds serve, Borys breaks serve, Borys holds serve, Borys breaks serve: $3$ breaks. </li></ul>
