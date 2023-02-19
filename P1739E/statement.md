## Description

<div><p>Consider a hallway, which can be represented as the matrix with $2$ rows and $n$ columns. Let's denote the cell on the intersection of the $i$-th row and the $j$-th column as $(i, j)$. The distance between the cells $(i_1, j_1)$ and $(i_2, j_2)$ is $|i_1 - i_2| + |j_1 - j_2|$.</p><p>There is a cleaning robot in the cell $(1, 1)$. Some cells of the hallway are clean, other cells are dirty (the cell with the robot is clean). You want to clean the hallway, so you are going to launch the robot to do this.</p><p>After the robot is launched, it works as follows. While at least one cell is dirty, the robot chooses <span class="tex-font-style-bf">the closest (to its current cell) cell</span> among those which are dirty, moves there and cleans it (so the cell is no longer dirty). After cleaning a cell, the robot again finds the closest dirty cell <span class="tex-font-style-bf">to its current cell</span>, and so on. This process repeats until the whole hallway is clean.</p><p>However, there is a critical bug in the robot's program. If at some moment, there are multiple closest (to the robot's current position) dirty cells, the robot malfunctions.</p><p>You want to clean the hallway in such a way that the robot doesn't malfunction. <span class="tex-font-style-bf">Before launching the robot</span>, you can clean some (possibly zero) of the dirty cells yourself. However, you don't want to do too much dirty work yourself while you have this nice, smart (yet buggy) robot to do this. Note that you cannot make a clean cell dirty.</p><p>Calculate the maximum possible number of cells you can leave dirty before launching the robot, so that it doesn't malfunction.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of columns in the hallway.</p><p>Then two lines follow, denoting the $1$-st and the $2$-nd row of the hallway. These lines contain $n$ characters each, where <span class="tex-font-style-tt">0</span> denotes a clean cell and <span class="tex-font-style-tt">1</span> denotes a dirty cell. The starting cell of the robot $(1, 1)$ is clean.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the maximum possible number of cells you can leave dirty before launching the robot, so that it doesn't malfunction.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of columns in the hallway.</p><p>Then two lines follow, denoting the $1$-st and the $2$-nd row of the hallway. These lines contain $n$ characters each, where <span class="tex-font-style-tt">0</span> denotes a clean cell and <span class="tex-font-style-tt">1</span> denotes a dirty cell. The starting cell of the robot $(1, 1)$ is clean.</p>

## Output

<p>Print one integer&nbsp;— the maximum possible number of cells you can leave dirty before launching the robot, so that it doesn't malfunction.</p>





```input1
2
01
11
```




```input2
2
01
01
```




```input3
4
0101
1011
```




```input4
4
0000
0000
```




```input5
5
00011
10101
```




```input6
6
011111
111111
```




```input7
10
0101001010
1010100110
```




```output1
2
```




```output2
2
```




```output3
4
```




```output4
0
```




```output5
4
```




```output6
8
```




```output7
6
```



## Note

<p>In the first example, you can clean the cell $(1, 2)$, so the path of the robot is $(1, 1) \rightarrow (2, 1) \rightarrow (2, 2)$.</p><p>In the second example, you can leave the hallway as it is, so the path of the robot is $(1, 1) \rightarrow (1, 2) \rightarrow (2, 2)$.</p><p>In the third example, you can clean the cell $(1, 2)$, so the path of the robot is $(1, 1) \rightarrow (2, 1) \rightarrow (2, 3) \rightarrow (2, 4) \rightarrow (1, 4)$.</p><p>In the fourth example, the hallway is already clean. Maybe you have launched the robot earlier?</p>
