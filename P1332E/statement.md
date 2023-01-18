## Description

<div><p>Alice has got addicted to a game called Sirtet recently.</p><p>In Sirtet, player is given an $n \times m$ grid. Initially $a_{i,j}$ cubes are stacked up in the cell $(i,j)$. Two cells are called adjacent if they share a side. Player can perform the following operations: </p><ul> <li> stack up one cube in two <span class="tex-font-style-bf">adjacent</span> cells; </li><li> stack up two cubes in one cell. </li></ul><p>Cubes mentioned above are identical in height.</p><p>Here is an illustration of the game. States on the right are obtained by performing one of the above operations on the state on the left, and grey cubes are added due to the operation.</p><center> <img class="tex-graphics" src="file://TV29hKZz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Player's goal is to <span class="tex-font-style-bf">make the height of all cells the same</span> (i.e. so that each cell has the same number of cubes in it) using above operations. </p><p>Alice, however, has found out that on some starting grids she may never reach the goal no matter what strategy she uses. Thus, she is wondering the number of initial grids such that </p><ul> <li> $L \le a_{i,j} \le R$ for all $1 \le i \le n$, $1 \le j \le m$; </li><li> player can reach the goal using above operations. </li></ul><p>Please help Alice with it. Notice that the answer might be large, please output the desired value modulo $998,244,353$.</p></div><div class="input-specification"><p>The only line contains four integers $n$, $m$, $L$ and $R$ ($1\le n,m,L,R \le 10^9$, $L \le R$, $n \cdot m \ge 2$).</p></div><div class="output-specification"><p>Output one integer, representing the desired answer modulo $998,244,353$.</p></div>

## Input

<p>The only line contains four integers $n$, $m$, $L$ and $R$ ($1\le n,m,L,R \le 10^9$, $L \le R$, $n \cdot m \ge 2$).</p>

## Output

<p>Output one integer, representing the desired answer modulo $998,244,353$.</p>





```input1
2 2 1 1
```




```input2
1 2 1 2
```




```output1
1
```




```output2
2
```



## Note

<p>In the first sample, the only initial grid that satisfies the requirements is $a_{1,1}=a_{2,1}=a_{1,2}=a_{2,2}=1$. Thus the answer should be $1$.</p><p>In the second sample, initial grids that satisfy the requirements are $a_{1,1}=a_{1,2}=1$ and $a_{1,1}=a_{1,2}=2$. Thus the answer should be $2$.</p>
