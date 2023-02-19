## Description

<div><p>Stanley and Megan decided to shop in the "Crossmarket" grocery store, which can be represented as a matrix with $n$ rows and $m$ columns. </p><p>Stanley and Megan can move to an adjacent cell using $1$ unit of power. Two cells are considered adjacent if they share an edge. To speed up the shopping process, Megan brought her portals with her, and she leaves one in each cell she visits (if there is no portal yet). If a person (Stanley or Megan) is in a cell with a portal, that person can use $1$ unit of power to teleport to any other cell with a portal, including Megan's starting cell.</p><p>They decided to split up: Stanley will go from the upper-left cell (cell with coordinates $(1, 1)$) to the lower-right cell (cell with coordinates $(n, m)$), whilst Megan needs to get from the lower-left cell (cell with coordinates $(n, 1)$) to the upper-right cell (cell with coordinates $(1, m)$).</p><p>What is the minimum total energy needed for them both to do that?</p><p>Note that they can choose the time they move. Time does not affect energy.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The only line in the test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^5$).</p></div><div class="output-specification"><p>For each test case print a single integer on a new line – the answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The only line in the test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^5$).</p>

## Output

<p>For each test case print a single integer on a new line – the answer.</p>





```input1|2,4,6,8
7
7 5
5 7
1 1
100000 100000
57 228
1 5
5 1
```




```output1
15
15
0
299998
340
5
5
```



## Note

<center> <img class="tex-graphics" src="file://cRqlCd0M.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the first test case they can stick to the following plan: </p><ol> <li> Megan (red circle) moves to the cell $(7, 3)$. Then she goes to the cell $(1, 3)$, and Stanley (blue circle) does the same. </li><li> Stanley uses the portal in that cell (cells with portals are grey) to get to the cell $(7, 3)$. Then he moves to his destination&nbsp;— cell $(7, 5)$. </li><li> Megan also finishes her route and goes to the cell $(1, 5)$. </li></ol><p>The total energy spent is $(2 + 6) + (2 + 1 + 2) + (2)= 15$, which is our final answer.</p>
