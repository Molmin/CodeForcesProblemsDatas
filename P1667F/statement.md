## Description

<div><p>You are given a rectangular grid with $n$ rows and $m$ columns. $n$ and $m$ are divisible by $4$. Some of the cells are already colored black or white. It is guaranteed that no two colored cells share a corner or an edge.</p><p>Color the remaining cells in a way that both the black and the white cells becomes orthogonally connected or determine that it is impossible.</p><p>Consider a graph, where the black cells are the nodes. Two nodes are adjacent if the corresponding cells share an edge. If the described graph is connected, the black cells are orthogonally connected. Same for white cells.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line of the input contains a single integer $t$ ($1 \le t \le 4000$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ ($8 \le n, m \le 500$, $n$ and $m$ are divisible by $4$) — the number of rows and columns.</p><p>Each of the next $n$ lines contains $m$ characters. Each character is either '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">W</span>' or '<span class="tex-font-style-tt">.</span>', representing black, white or empty cell respectively. Two colored (black or white) cell does not share a corner or an edge.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $250\,000$.</p></div><div class="output-specification"><p>For each testcase print "<span class="tex-font-style-tt">NO</span>" if there is no solution, otherwise print "<span class="tex-font-style-tt">YES</span>" and a grid with the same format. If there are multiple solutions, you can print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line of the input contains a single integer $t$ ($1 \le t \le 4000$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ ($8 \le n, m \le 500$, $n$ and $m$ are divisible by $4$) — the number of rows and columns.</p><p>Each of the next $n$ lines contains $m$ characters. Each character is either '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">W</span>' or '<span class="tex-font-style-tt">.</span>', representing black, white or empty cell respectively. Two colored (black or white) cell does not share a corner or an edge.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $250\,000$.</p>

## Output

<p>For each testcase print "<span class="tex-font-style-tt">NO</span>" if there is no solution, otherwise print "<span class="tex-font-style-tt">YES</span>" and a grid with the same format. If there are multiple solutions, you can print any.</p>





```input1
4
8 8
.W.W....
.....B.W
.W.W....
.....W.W
B.B.....
....B.B.
B.W.....
....B.B.
8 8
B.W..B.W
........
W.B..W.B
........
........
B.W..B.W
........
W.B..W.B
8 12
W.B.........
....B...B.W.
B.B.........
....B...B.B.
.B..........
........B...
.W..B.B...W.
............
16 16
.W............W.
...W..W..W.W....
.B...........B.W
....W....W......
W......B....W.W.
..W.......B.....
....W...W....B.W
.W....W....W....
...B...........W
W.....W...W..B..
..W.W...W......B
............W...
.W.B...B.B....B.
.....W.....W....
..W......W...W..
W...W..W...W...W
```




```output1
YES
BWWWWWWW
BWBBBBBW
BWBWWWBW
BWBWBWBW
BWBWBWBW
BWBBBWBW
BWWWWWBW
BBBBBBBW
NO
YES
WWBBBBBBBBBB
BWWWBBBBBBWB
BBBWBBBWWWWB
BBBWBBBWBBBB
BBBWBBBWBBBB
BBBWWWWWBBBB
BWWWBBBWWWWB
BBBBBBBBBBBB
YES
WWWWWWWWWWWWWWWW
WWWWWWWWWWWWWWWW
WBBBBBBBBBBBBBWW
WBBBWBWWWWBWWBWW
WBBWWBBBWWBWWBWW
WBWWWBWWWWBWWBWW
WBBWWBBBWWBWWBWW
WWBWWWWWWWWWWWWW
WWBBBBBBBBBBBBWW
WBBBWWWBWWWBWBWW
WWWBWBBBWBBBWBBB
WWWBWBWWWWWBWWBW
WWWBWBBBWBBBWWBW
WWWWWWWWWWWWWWWW
WWWWWWWWWWWWWWWW
WWWWWWWWWWWWWWWW
```



## Note

<p>Solution for test case 1: </p><center> <img class="tex-graphics" src="file://ABAVRJNh.png" style="max-width: 100.0%;max-height: 100.0%;">   </center><p>Test case 2: one can see that the black and the white part can't be connected in the same time. So the answer is "<span class="tex-font-style-tt">NO</span>". </p>
