## Description

<div><p>There is a grid with $n$ rows and $m$ columns. Some cells are colored black, and the rest of the cells are colored white.</p><p>In one operation, you can select some <span class="tex-font-style-bf">black</span> cell and do <span class="tex-font-style-bf">exactly one</span> of the following: </p><ul> <li> color all cells in its row black, or </li><li> color all cells in its column black. </li></ul><p>You are given two integers $r$ and $c$. Find the minimum number of operations required to make the cell in row $r$ and column $c$ black, or determine that it is impossible.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains four integers $n$, $m$, $r$, and $c$ ($1 \leq n, m \leq 50$; $1 \leq r \leq n$; $1 \leq c \leq m$)&nbsp;— the number of rows and the number of columns in the grid, and the row and column of the cell you need to turn black, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>'&nbsp;— a black and a white cell, respectively.</p></div><div class="output-specification"><p>For each test case, if it is impossible to make the cell in row $r$ and column $c$ black, output $-1$. </p><p>Otherwise, output a single integer&nbsp;— the minimum number of operations required to make the cell in row $r$ and column $c$ black. </p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains four integers $n$, $m$, $r$, and $c$ ($1 \leq n, m \leq 50$; $1 \leq r \leq n$; $1 \leq c \leq m$)&nbsp;— the number of rows and the number of columns in the grid, and the row and column of the cell you need to turn black, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>'&nbsp;— a black and a white cell, respectively.</p>

## Output

<p>For each test case, if it is impossible to make the cell in row $r$ and column $c$ black, output $-1$. </p><p>Otherwise, output a single integer&nbsp;— the minimum number of operations required to make the cell in row $r$ and column $c$ black. </p>





```input1
9
3 5 1 4
WBWWW
BBBWB
WWBBB
4 3 2 1
BWW
BBW
WBB
WWB
2 3 2 2
WWW
WWW
2 2 1 1
WW
WB
5 9 5 9
WWWWWWWWW
WBWBWBBBW
WBBBWWBWW
WBWBWBBBW
WWWWWWWWW
1 1 1 1
B
1 1 1 1
W
1 2 1 1
WB
2 1 1 1
W
B
```




```output1
1
0
-1
2
2
0
-1
1
1
```



## Note

<p>The first test case is pictured below.</p><center> <img class="tex-graphics" src="file://LvpBlccd.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We can take the black cell in row $1$ and column $2$, and make all cells in its row black. Therefore, the cell in row $1$ and column $4$ will become black.</p><center> <img class="tex-graphics" src="file://NWXidJwd.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second test case, the cell in row $2$ and column $1$ is already black.</p><p>In the third test case, it is impossible to make the cell in row $2$ and column $2$ black.</p><p>The fourth test case is pictured below.</p><center> <img class="tex-graphics" src="file://9Y77ufXw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We can take the black cell in row $2$ and column $2$ and make its column black. </p><center> <img class="tex-graphics" src="file://0G02eL2X.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Then, we can take the black cell in row $1$ and column $2$ and make its row black. </p><center> <img class="tex-graphics" src="file://27XWsNl1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Therefore, the cell in row $1$ and column $1$ will become black.</p>
