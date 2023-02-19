## Description

<div><p>You found a map of a weirdly shaped labyrinth. The map is a grid, consisting of $n$ rows and $n$ columns. The rows of the grid are numbered from $1$ to $n$ from bottom to top. The columns of the grid are numbered from $1$ to $n$ from left to right.</p><p>The labyrinth has $n$ layers. The first layer is the bottom left corner (cell $(1, 1)$). The second layer consists of all cells that are in the grid and adjacent to the first layer by a side or a corner. The third layer consists of all cells that are in the grid and adjacent to the second layer by a side or a corner. And so on. </p><p>The labyrinth with $5$ layers, for example, is shaped as follows: </p><center> <img class="tex-graphics" src="file://6uhiNHp0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The layers are separated from one another with walls. However, there are doors in these walls.</p><p>Each layer (except for layer $n$) has exactly two doors to the next layer. One door is placed on the top wall of the layer and another door is placed on the right wall of the layer. For each layer from $1$ to $n-1$ you are given positions of these two doors. The doors can be passed in both directions: either from layer $i$ to layer $i+1$ or from layer $i+1$ to layer $i$.</p><p>If you are standing in some cell, you can move to an adjacent by a side cell if a wall doesn't block your move (e.g. you can't move to a cell in another layer if there is no door between the cells).</p><p>Now you have $m$ queries of sort: what's the minimum number of moves one has to make to go from cell $(x_1, y_1)$ to cell $(x_2, y_2)$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of layers in the labyrinth.</p><p>The $i$-th of the next $n-1$ lines contains four integers $d_{1,x}, d_{1,y}, d_{2,x}$ and $d_{2,y}$ ($1 \le d_{1,x}, d_{1,y}, d_{2,x}, d_{2,y} \le n$)&nbsp;— the coordinates of the doors. Both cells are on the $i$-th layer. The first cell is adjacent to the top wall of the $i$-th layer by a side&nbsp;— that side is where the door is. The second cell is adjacent to the right wall of the $i$-th layer by a side&nbsp;— that side is where the door is.</p><p>The next line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>The $j$-th of the next $m$ lines contains four integers $x_1, y_1, x_2$ and $y_2$ ($1 \le x_1, y_1, x_2, y_2 \le n$)&nbsp;— the coordinates of the cells in the $j$-th query.</p></div><div class="output-specification"><p>For each query, print a single integer&nbsp;— the minimum number of moves one has to make to go from cell $(x_1, y_1)$ to cell $(x_2, y_2)$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of layers in the labyrinth.</p><p>The $i$-th of the next $n-1$ lines contains four integers $d_{1,x}, d_{1,y}, d_{2,x}$ and $d_{2,y}$ ($1 \le d_{1,x}, d_{1,y}, d_{2,x}, d_{2,y} \le n$)&nbsp;— the coordinates of the doors. Both cells are on the $i$-th layer. The first cell is adjacent to the top wall of the $i$-th layer by a side&nbsp;— that side is where the door is. The second cell is adjacent to the right wall of the $i$-th layer by a side&nbsp;— that side is where the door is.</p><p>The next line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>The $j$-th of the next $m$ lines contains four integers $x_1, y_1, x_2$ and $y_2$ ($1 \le x_1, y_1, x_2, y_2 \le n$)&nbsp;— the coordinates of the cells in the $j$-th query.</p>

## Output

<p>For each query, print a single integer&nbsp;— the minimum number of moves one has to make to go from cell $(x_1, y_1)$ to cell $(x_2, y_2)$.</p>





```input1
2
1 1 1 1
10
1 1 1 1
1 1 1 2
1 1 2 1
1 1 2 2
1 2 1 2
1 2 2 1
1 2 2 2
2 1 2 1
2 1 2 2
2 2 2 2
```




```input2
4
1 1 1 1
2 1 2 2
3 2 1 3
5
2 4 4 3
4 4 3 3
1 2 3 3
2 2 4 4
1 4 2 3
```




```output1
0
1
1
2
0
2
1
0
1
0
```




```output2
3
4
3
6
2
```



## Note

<p>Here is the map of the labyrinth from the second example. The doors are marked red.</p><center> <img class="tex-graphics" src="file://Y7R7CgXR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
