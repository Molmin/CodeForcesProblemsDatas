## Description

<div><p>Nauuo is a girl who loves playing chess.</p><p>One day she invented a game by herself which needs $n$ chess pieces to play on a $m\times m$ chessboard. The rows and columns are numbered from $1$ to $m$. We denote a cell on the intersection of the $r$-th row and $c$-th column as $(r,c)$.</p><p>The game's goal is to place $n$ chess pieces numbered from $1$ to $n$ on the chessboard, the $i$-th piece lies on $(r_i,\,c_i)$, while the following rule is satisfied: for all pairs of pieces $i$ and $j$, $|r_i-r_j|+|c_i-c_j|\ge|i-j|$. Here $|x|$ means the absolute value of $x$.</p><p>However, Nauuo discovered that sometimes she couldn't find a solution because the chessboard was too small.</p><p>She wants to find the <span class="tex-font-style-bf">smallest</span> chessboard on which she can put $n$ pieces according to the rules.</p><p>She also wonders how to place the pieces on such a chessboard. Can you help her?</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1\le n\le 1000$) — the number of chess pieces for the game.</p></div><div class="output-specification"><p>The first line contains a single integer — the minimum value of $m$, where $m$ is the length of sides of the suitable chessboard.</p><p>The $i$-th of the next $n$ lines contains two integers $r_i$ and $c_i$ ($1\le r_i,c_i\le m$) — the coordinates of the $i$-th chess piece.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1\le n\le 1000$) — the number of chess pieces for the game.</p>

## Output

<p>The first line contains a single integer — the minimum value of $m$, where $m$ is the length of sides of the suitable chessboard.</p><p>The $i$-th of the next $n$ lines contains two integers $r_i$ and $c_i$ ($1\le r_i,c_i\le m$) — the coordinates of the $i$-th chess piece.</p><p>If there are multiple answers, print any.</p>





```input1
2
```




```input2
4
```




```output1
2
1 1
1 2
```




```output2
3
1 1
1 3
3 1
3 3
```



## Note

<p>In the first example, you can't place the two pieces on a $1\times1$ chessboard without breaking the rule. But you can place two pieces on a $2\times2$ chessboard like this:</p><p><img class="tex-graphics" src="file://yB3cc0ws.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second example, you can't place four pieces on a $2\times2$ chessboard without breaking the rule. For example, if you place the pieces like this:</p><p><img class="tex-graphics" src="file://Aj58cTgq.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>then $|r_1-r_3|+|c_1-c_3|=|1-2|+|1-1|=1$, $|1-3|=2$, $1&lt;2$; and $|r_1-r_4|+|c_1-c_4|=|1-2|+|1-2|=2$, $|1-4|=3$, $2&lt;3$. It doesn't satisfy the rule.</p><p>However, on a $3\times3$ chessboard, you can place four pieces like this:</p><p><img class="tex-graphics" src="file://oEqabix6.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
