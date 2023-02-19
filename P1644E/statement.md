## Description

<div><p>Consider a grid of size $n \times n$. The rows are numbered top to bottom from $1$ to $n$, the columns are numbered left to right from $1$ to $n$.</p><p>The robot is positioned in a cell $(1, 1)$. It can perform two types of moves:</p><ul> <li> <span class="tex-font-style-tt">D</span>&nbsp;— move one cell down; </li><li> <span class="tex-font-style-tt">R</span>&nbsp;— move one cell right. </li></ul><p>The robot is not allowed to move outside the grid.</p><p>You are given a sequence of moves $s$&nbsp;— the initial path of the robot. This path doesn't lead the robot outside the grid.</p><p>You are allowed to perform an arbitrary number of modifications to it (possibly, zero). With one modification, you can duplicate one move in the sequence. That is, replace a single occurrence of <span class="tex-font-style-tt">D</span> with <span class="tex-font-style-tt">DD</span> or a single occurrence of <span class="tex-font-style-tt">R</span> with <span class="tex-font-style-tt">RR</span>.</p><p>Count the number of cells such that there exists at least one sequence of modifications that the robot visits this cell on the modified path and doesn't move outside the grid.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains the single integer $n$ ($2 \le n \le 10^8$)&nbsp;— the number of rows and columns in the grid.</p><p>The second line of each testcase contains a non-empty string $s$, consisting only of characters <span class="tex-font-style-tt">D</span> and <span class="tex-font-style-tt">R</span>,&nbsp;— the initial path of the robot. This path doesn't lead the robot outside the grid.</p><p>The total length of strings $s$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the number of cells such that there exists at least one sequence of modifications that the robot visits this cell on the modified path and doesn't move outside the grid.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains the single integer $n$ ($2 \le n \le 10^8$)&nbsp;— the number of rows and columns in the grid.</p><p>The second line of each testcase contains a non-empty string $s$, consisting only of characters <span class="tex-font-style-tt">D</span> and <span class="tex-font-style-tt">R</span>,&nbsp;— the initial path of the robot. This path doesn't lead the robot outside the grid.</p><p>The total length of strings $s$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the number of cells such that there exists at least one sequence of modifications that the robot visits this cell on the modified path and doesn't move outside the grid.</p>





```input1
3
4
RD
5
DRDRDRDR
3
D
```




```output1
13
9
3
```



## Note

<p>In the first testcase, it's enough to consider the following modified paths: </p><ul> <li> <span class="tex-font-style-tt">RD</span> $\rightarrow$ <span class="tex-font-style-tt">RRD</span> $\rightarrow$ <span class="tex-font-style-tt">RRRD</span> $\rightarrow$ <span class="tex-font-style-tt">RRRDD</span> $\rightarrow$ <span class="tex-font-style-tt">RRRDDD</span>&nbsp;— this path visits cells $(1, 1)$, $(1, 2)$, $(1, 3)$, $(1, 4)$, $(2, 4)$, $(3, 4)$ and $(4, 4)$; </li><li> <span class="tex-font-style-tt">RD</span> $\rightarrow$ <span class="tex-font-style-tt">RRD</span> $\rightarrow$ <span class="tex-font-style-tt">RRDD</span> $\rightarrow$ <span class="tex-font-style-tt">RRDDD</span>&nbsp;— this path visits cells $(1, 1)$, $(1, 2)$, $(1, 3)$, $(2, 3)$, $(3, 3)$ and $(4, 3)$; </li><li> <span class="tex-font-style-tt">RD</span> $\rightarrow$ <span class="tex-font-style-tt">RDD</span> $\rightarrow$ <span class="tex-font-style-tt">RDDD</span>&nbsp;— this path visits cells $(1, 1)$, $(1, 2)$, $(2, 2)$, $(3, 2)$ and $(4, 2)$. </li></ul><p>Thus, the cells that are visited on at least one modified path are: $(1, 1)$, $(1, 2)$, $(1, 3)$, $(1, 4)$, $(2, 2)$, $(2, 3)$, $(2, 4)$, $(3, 2)$, $(3, 3)$, $(3, 4)$, $(4, 2)$, $(4, 3)$ and $(4, 4)$.</p><p>In the second testcase, there is no way to modify the sequence without moving the robot outside the grid. So the only visited cells are the ones that are visited on the path <span class="tex-font-style-tt">DRDRDRDR</span>.</p><p>In the third testcase, the cells that are visited on at least one modified path are: $(1, 1)$, $(2, 1)$ and $(3, 1)$.</p><p>Here are the cells for all testcases:</p><center> <img class="tex-graphics" src="file://UtxE1m58.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
