## Description

<div><p>After watching the new <span class="tex-font-style-striked">over-rated</span> series Squid Game, Mashtali and Soroush decided to hold their own Squid Games! Soroush agreed to be the host and will provide money for the winner's prize, and Mashtali became the Front Man!</p><p>$m$ players registered to play in the games to win the great prize, but when Mashtali found out how huge the winner's prize is going to be, he decided to <span class="tex-font-style-striked">kill</span> eliminate all the players so he could take the money for himself!</p><p>Here is how evil Mashtali is going to eliminate players:</p><p>There is an unrooted tree with $n$ vertices. Every player has $2$ special vertices $x_i$ and $y_i$.</p><p>In one operation, Mashtali can choose any vertex $v$ of the tree. Then, for each remaining player $i$ he finds a vertex $w$ on the simple path from $x_i$ to $y_i$, which is the closest to $v$. If $w\ne x_i$ and $w\ne y_i$, player $i$ will be eliminated.</p><p>Now Mashtali wondered: "What is the minimum number of operations I should perform so that I can remove every player from the game and take the money for myself?"</p><p>Since he was only thinking about the money, he couldn't solve the problem by himself and asked for your help!</p></div><div class="input-specification"><p>The first line contains $2$ integer $n$ and $m$ $(1 \le n, m \le 3 \cdot 10^5)$&nbsp;— the number of vertices of the tree and the number of players.</p><p>The second line contains $n-1$ integers $par_2, par_3, \ldots, par_n$ $(1 \le par_i &lt; i)$&nbsp;— denoting an edge between node $i$ and $par_i$.</p><p>The $i$-th of the following $m$ lines contains two integers $x_i$ and $y_i$ $(1 \le x_i, y_i \le n, x_i \ne y_i)$&nbsp;— the special vertices of the $i$-th player.</p></div><div class="output-specification"><p>Print the minimum number of operations Mashtali has to perform.</p><p>If there is no way for Mashtali to eliminate all the players, print $-1$.</p></div>

## Input

<p>The first line contains $2$ integer $n$ and $m$ $(1 \le n, m \le 3 \cdot 10^5)$&nbsp;— the number of vertices of the tree and the number of players.</p><p>The second line contains $n-1$ integers $par_2, par_3, \ldots, par_n$ $(1 \le par_i &lt; i)$&nbsp;— denoting an edge between node $i$ and $par_i$.</p><p>The $i$-th of the following $m$ lines contains two integers $x_i$ and $y_i$ $(1 \le x_i, y_i \le n, x_i \ne y_i)$&nbsp;— the special vertices of the $i$-th player.</p>

## Output

<p>Print the minimum number of operations Mashtali has to perform.</p><p>If there is no way for Mashtali to eliminate all the players, print $-1$.</p>





```input1
6 3
1 1 1 4 4
1 5
3 4
2 6
```




```input2
5 3
1 1 3 3
1 2
1 4
1 5
```




```output1
2
```




```output2
-1
```



## Note

<p>Explanation for the first sample:</p><center> <img class="tex-graphics" src="file://j9TxpSGx.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">In the first operation, Mashtali can choose vertex $1$ and eliminate players with colors red and blue. In the second operation, he can choose vertex $6$ and eliminate the player with orange color.</span> </center><p>In the second sample, Mashtali can't eliminate the first player.</p>
