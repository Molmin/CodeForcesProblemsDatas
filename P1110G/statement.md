## Description

<div><p>The tic-tac-toe game is starting on a tree of $n$ vertices. Some vertices are already colored in white while the remaining are uncolored.</p><p>There are two players&nbsp;— white and black. The players make moves alternatively. The white player starts the game. In his turn, a player must select one uncolored vertex and paint it in his color.</p><p>The player wins if he paints some path of three vertices in his color. In case all vertices are colored and neither player won, the game ends in a draw.</p><p>Could you please find who will win the game or whether it ends as a draw, assuming both players play optimally? </p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 50\,000$)&nbsp;— the number of test cases. Then descriptions of $T$ test cases follow.</p><p>The first line of each test contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Each of the following $n - 1$ lines contains integers $v$, $u$ ($1 \le v, u \le n$) denoting an edge of the tree connecting vertices $v$ and $u$.</p><p>The last line of a test case contains a string of letters '<span class="tex-font-style-tt">W</span>' (for white) and '<span class="tex-font-style-tt">N</span>' (for not colored) of length $n$ denoting already colored vertices. Vertexes already colored in white are denoted as '<span class="tex-font-style-tt">W</span>'.</p><p>It's guaranteed that the given edges form a tree, that there is at least one uncolored vertex and that there is no path of three white vertices.</p><p>It's guaranteed that sum of all $n$ among all test cases is at most $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For every test case, print either "<span class="tex-font-style-tt">White</span>", "<span class="tex-font-style-tt">Draw</span>" or "<span class="tex-font-style-tt">Black</span>", depending on the result of the game.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 50\,000$)&nbsp;— the number of test cases. Then descriptions of $T$ test cases follow.</p><p>The first line of each test contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Each of the following $n - 1$ lines contains integers $v$, $u$ ($1 \le v, u \le n$) denoting an edge of the tree connecting vertices $v$ and $u$.</p><p>The last line of a test case contains a string of letters '<span class="tex-font-style-tt">W</span>' (for white) and '<span class="tex-font-style-tt">N</span>' (for not colored) of length $n$ denoting already colored vertices. Vertexes already colored in white are denoted as '<span class="tex-font-style-tt">W</span>'.</p><p>It's guaranteed that the given edges form a tree, that there is at least one uncolored vertex and that there is no path of three white vertices.</p><p>It's guaranteed that sum of all $n$ among all test cases is at most $5 \cdot 10^5$.</p>

## Output

<p>For every test case, print either "<span class="tex-font-style-tt">White</span>", "<span class="tex-font-style-tt">Draw</span>" or "<span class="tex-font-style-tt">Black</span>", depending on the result of the game.</p>





```input1
2
4
1 2
1 3
1 4
NNNW
5
1 2
2 3
3 4
4 5
NNNNN
```




```output1
White
Draw
```



## Note

<p>In the first example, vertex $4$ is already colored in white. The white player can win by coloring the vertex $1$ in white first and the remaining vertex on his second turn. The process is illustrated with the pictures below.</p><center> <img class="tex-graphics" src="file://CMyZpFtn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, we can show that no player can enforce their victory.</p>
