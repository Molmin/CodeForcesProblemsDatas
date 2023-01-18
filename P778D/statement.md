## Description

<div><p>Peter decided to lay a parquet in the room of size <span class="tex-span"><i>n</i> × <i>m</i></span>, the parquet consists of tiles of size <span class="tex-span">1 × 2</span>. When the workers laid the parquet, it became clear that the tiles pattern looks not like Peter likes, and workers will have to re-lay it.</p><p>The workers decided that removing entire parquet and then laying it again is very difficult task, so they decided to make such an operation every hour: remove two tiles, which form a <span class="tex-span">2 × 2</span> square, rotate them 90 degrees and put them back on the same place.</p><center> <img class="tex-graphics" src="file://sUj6j1Pi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>They have no idea how to obtain the desired configuration using these operations, and whether it is possible at all.</p><p>Help Peter to make a plan for the workers or tell that it is impossible. The plan should contain at most <span class="tex-span">100 000</span> commands.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, size of the room (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>). At least one of them is even number.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each, the description of the current configuration of the parquet tiles. Each character represents the position of the half-tile. Characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">D</span>' correspond to the left, right, upper and lower halves, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each, describing the desired configuration in the same format.</p></div><div class="output-specification"><p>In the first line output integer <span class="tex-span"><i>k</i></span>, the number of operations. In the next <span class="tex-span"><i>k</i></span> lines output description of operations. The operation is specified by coordinates (row and column) of the left upper half-tile on which the operation is performed.</p><p>If there is no solution, output <span class="tex-font-style-tt">-1</span> in the first line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, size of the room (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>). At least one of them is even number.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each, the description of the current configuration of the parquet tiles. Each character represents the position of the half-tile. Characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">D</span>' correspond to the left, right, upper and lower halves, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each, describing the desired configuration in the same format.</p>

## Output

<p>In the first line output integer <span class="tex-span"><i>k</i></span>, the number of operations. In the next <span class="tex-span"><i>k</i></span> lines output description of operations. The operation is specified by coordinates (row and column) of the left upper half-tile on which the operation is performed.</p><p>If there is no solution, output <span class="tex-font-style-tt">-1</span> in the first line.</p>





```input1
2 3
ULR
DLR
LRU
LRD

```




```input2
4 3
ULR
DLR
LRU
LRD
ULR
DUU
UDD
DLR
```




```output1
2
1 2
1 1

```




```output2
3
3 1
3 2
2 2
```



## Note

<p>In the first sample test first operation is to rotate two rightmost tiles, after this all tiles lie vertically. Second operation is to rotate two leftmost tiles, after this we will get desired configuration.</p><center> <img class="tex-graphics" src="file://uAd3daSn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
