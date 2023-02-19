## Description

<div><p>Emma loves playing with blocks. She has several cubic blocks of the same size that are numbered with <span class="tex-font-style-bf">distinct</span> integers written on them. She assembles towers from those blocks by stacking them vertically. </p><p>A configuration of her game is a set of towers that she has assembled from the blocks. Emma can perform two kinds of operations on a configuration of towers:</p><ul><li> <span class="tex-font-style-bf">Split</span> any tower with more than one block in it by taking any number of blocks from the top of the tower and moving them to a new tower keeping their order, so that the top block of the old tower becomes the top block of the new tower. As a result of this operation, the number of towers increases by one.</li><li> <span class="tex-font-style-bf">Combine</span> any two towers by moving blocks from one tower on top of the other tower in the same order. As a result of this operation, the number of towers decreases by one.</li></ul><p>Emma wants to stack all the blocks into a single tower so that all blocks come in order sorted by the numbers&nbsp;— from the block with the minimal number at the top to the block with the maximal number at the bottom. Emma wants to do as little of splitting and combining operations as possible. Your task is to find the minimal number of operations she has to make and output how many splits and combines are needed. </p></div><div class="input-specification"><p>The first line of the input file contains an integer $n$ ($1 \le n \le 10\,000$)&nbsp;— the number of towers in the initial configuration. Next $n$ lines describe towers. Each tower $i$ is described by a line that starts with the number $k_i$ ($k_i \ge 1$; $\sum_1^n{k_i} \le 10\,000$)&nbsp;— the number of blocks in the tower, followed by $k_i$ numbers $b_{i,j}$ ($1 \le b_{i,j} \le 10^9$)&nbsp;— numbers written on the blocks in the $i$-th tower, listed from top to bottom. All block numbers listed in the input are different. </p></div><div class="output-specification"><p>Output a line with two integers $s$ and $c$&nbsp;— the number of split and combine operations Emma should make to get a single tower with blocks sorted by their numbers, so that the total number of operations is minimized.</p></div>

## Input

<p>The first line of the input file contains an integer $n$ ($1 \le n \le 10\,000$)&nbsp;— the number of towers in the initial configuration. Next $n$ lines describe towers. Each tower $i$ is described by a line that starts with the number $k_i$ ($k_i \ge 1$; $\sum_1^n{k_i} \le 10\,000$)&nbsp;— the number of blocks in the tower, followed by $k_i$ numbers $b_{i,j}$ ($1 \le b_{i,j} \le 10^9$)&nbsp;— numbers written on the blocks in the $i$-th tower, listed from top to bottom. All block numbers listed in the input are different. </p>

## Output

<p>Output a line with two integers $s$ and $c$&nbsp;— the number of split and combine operations Emma should make to get a single tower with blocks sorted by their numbers, so that the total number of operations is minimized.</p>





```input1
2
3 3 5 8
2 9 2
```




```output1
1 2
```



## Note

<p>The example needs the following operations (1 split and 2 combines).</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://XNzYLHX6.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://IBNgLq1W.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://YnBJOWNC.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://knKhjqTJ.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr><tr><td class="tex-tabular-text-align-center">Initial</td><td class="tex-tabular-text-align-center">Split last</td><td class="tex-tabular-text-align-center">Combined 2nd onto 1st</td><td class="tex-tabular-text-align-center">Combined 1st onto 2nd</td></tr></tbody></table><p></p>
