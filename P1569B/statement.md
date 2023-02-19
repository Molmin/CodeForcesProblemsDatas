## Description

<div><p>A chess tournament will be held soon, where $n$ chess players will take part. Every participant will play one game against every other participant. Each game ends in either a win for one player and a loss for another player, or a draw for both players.</p><p>Each of the players has their own expectations about the tournament, they can be one of two types:</p><ol> <li> a player wants not to lose any game (i. e. finish the tournament with <span class="tex-font-style-bf">zero losses</span>); </li><li> a player wants to win at least one game. </li></ol><p>You have to determine if there exists an outcome for all the matches such that all the players meet their expectations. If there are several possible outcomes, print any of them. If there are none, report that it's impossible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($2 \le n \le 50$)&nbsp;— the number of chess players.</p><p>The second line contains the string $s$ ($|s| = n$; $s_i \in \{1, 2\}$). If $s_i = 1$, then the $i$-th player has expectations of the first type, otherwise of the second type.</p></div><div class="output-specification"><p>For each test case, print the answer in the following format:</p><p>In the first line, print <span class="tex-font-style-tt">NO</span> if it is impossible to meet the expectations of all players.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span>, and the matrix of size $n \times n$ in the next $n$ lines.</p><p>The matrix element in the $i$-th row and $j$-th column should be equal to:</p><ul> <li> <span class="tex-font-style-tt">+</span>, if the $i$-th player won in a game against the $j$-th player; </li><li> <span class="tex-font-style-tt">-</span>, if the $i$-th player lost in a game against the $j$-th player; </li><li> <span class="tex-font-style-tt">=</span>, if the $i$-th and $j$-th players' game resulted in a draw; </li><li> <span class="tex-font-style-tt">X</span>, if $i = j$. </li></ul></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($2 \le n \le 50$)&nbsp;— the number of chess players.</p><p>The second line contains the string $s$ ($|s| = n$; $s_i \in \{1, 2\}$). If $s_i = 1$, then the $i$-th player has expectations of the first type, otherwise of the second type.</p>

## Output

<p>For each test case, print the answer in the following format:</p><p>In the first line, print <span class="tex-font-style-tt">NO</span> if it is impossible to meet the expectations of all players.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span>, and the matrix of size $n \times n$ in the next $n$ lines.</p><p>The matrix element in the $i$-th row and $j$-th column should be equal to:</p><ul> <li> <span class="tex-font-style-tt">+</span>, if the $i$-th player won in a game against the $j$-th player; </li><li> <span class="tex-font-style-tt">-</span>, if the $i$-th player lost in a game against the $j$-th player; </li><li> <span class="tex-font-style-tt">=</span>, if the $i$-th and $j$-th players' game resulted in a draw; </li><li> <span class="tex-font-style-tt">X</span>, if $i = j$. </li></ul>





```input1
3
3
111
2
21
4
2122
```




```output1
YES
X==
=X=
==X
NO
YES
X--+
+X++
+-X-
--+X
```


