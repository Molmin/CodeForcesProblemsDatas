## Description

<div><p>There are many sunflowers in the Garden of the Sun.</p><p>Garden of the Sun is a rectangular table with $n$ rows and $m$ columns, where the cells of the table are farmlands. All of the cells grow a sunflower on it. Unfortunately, one night, the lightning stroke some (possibly zero) cells, and sunflowers on those cells were burned into ashes. In other words, those cells struck by the lightning became empty. Magically, <span class="tex-font-style-bf">any two empty cells have no common points</span> (neither edges nor corners).</p><p>Now the owner wants to remove some (possibly zero) sunflowers to reach the following two goals: </p><ul>  <li> When you are on an empty cell, you can walk to any other empty cell. In other words, those empty cells are connected.  </li><li> There is <span class="tex-font-style-bf">exactly one</span> simple path between any two empty cells. In other words, there is no cycle among the empty cells. </li></ul><p>You can walk from an empty cell to another if they share a common edge.</p><p>Could you please give the owner a solution that meets all her requirements?</p><p>Note that you are not allowed to plant sunflowers. You <span class="tex-font-style-bf">don't need</span> to minimize the number of sunflowers you remove. It can be shown that the answer always exists.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains two integers $n$, $m$ ($1 \le n,m \le 500$)&nbsp;— the number of rows and columns. </p><p>Each of the next $n$ lines contains $m$ characters. Each character is either '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">.</span>', representing an empty cell and a cell that grows a sunflower, respectively.</p><p>It is guaranteed that the sum of $n \cdot m$ for all test cases does not exceed $250\,000$.</p></div><div class="output-specification"><p>For each test case, print $n$ lines. Each should contain $m$ characters, representing one row of the table. Each character should be either '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">.</span>', representing an empty cell and a cell with a sunflower, respectively.</p><p>If there are multiple answers, you can print any. It can be shown that the answer always exists.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains two integers $n$, $m$ ($1 \le n,m \le 500$)&nbsp;— the number of rows and columns. </p><p>Each of the next $n$ lines contains $m$ characters. Each character is either '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">.</span>', representing an empty cell and a cell that grows a sunflower, respectively.</p><p>It is guaranteed that the sum of $n \cdot m$ for all test cases does not exceed $250\,000$.</p>

## Output

<p>For each test case, print $n$ lines. Each should contain $m$ characters, representing one row of the table. Each character should be either '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">.</span>', representing an empty cell and a cell with a sunflower, respectively.</p><p>If there are multiple answers, you can print any. It can be shown that the answer always exists.</p>





```input1
5
3 3
X.X
...
X.X
4 4
....
.X.X
....
.X.X
5 5
.X...
....X
.X...
.....
X.X.X
1 10
....X.X.X.
2 2
..
..
```




```output1
XXX
..X
XXX
XXXX
.X.X
.X..
.XXX
.X...
.XXXX
.X...
.X...
XXXXX
XXXXXXXXXX
..
..
```



## Note

<p>Let's use $(x,y)$ to describe the cell on $x$-th row and $y$-th column.</p><p>In the following pictures white, yellow, and blue cells stand for the cells that grow a sunflower, the cells lightning stroke, and the cells sunflower on which are removed, respectively.</p><p><img class="tex-graphics" src="file://E3kV7x1n.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the first test case, one possible solution is to remove sunflowers on $(1,2)$, $(2,3)$ and $(3 ,2)$. </p><p><img class="tex-graphics" src="file://YwinXaXd.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Another acceptable solution is to remove sunflowers on $(1,2)$, $(2,2)$ and $(3,2)$. </p><p><img class="tex-graphics" src="file://4pzl1Bw2.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>This output is considered wrong because there are 2 simple paths between any pair of cells (there is a cycle). For example, there are 2 simple paths between $(1,1)$ and $(3,3)$.</p><ol> <li> $(1,1)\to (1,2)\to (1,3)\to (2,3)\to (3,3)$<p> </p></li><li> $(1,1)\to (2,1)\to (3,1)\to (3,2)\to (3,3)$ </li></ol><p><img class="tex-graphics" src="file://cZmCUkn0.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>This output is considered wrong because you can't walk from $(1,1)$ to $(3,3)$.</p>
