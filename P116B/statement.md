## Description

<div><p>Once upon a time there were several little pigs and several wolves on a two-dimensional grid of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Each cell in this grid was either empty, containing one little pig, or containing one wolf.</p><p>A little pig and a wolf are adjacent if the cells that they are located at share a side. The little pigs are afraid of wolves, so there will be at most one wolf adjacent to each little pig. But each wolf may be adjacent to any number of little pigs.</p><p>They have been living peacefully for several years. But today the wolves got hungry. One by one, each wolf will choose one of the little pigs adjacent to it (if any), and eats the poor little pig. This process is not repeated. That is, each wolf will get to eat at most one little pig. Once a little pig gets eaten, it disappears and cannot be eaten by any other wolf.</p><p>What is the maximum number of little pigs that may be eaten by the wolves?</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10</span>) which denotes the number of rows and columns in our two-dimensional grid, respectively. Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each — that is the grid description. "<span class="tex-font-style-tt">.</span>" means that this cell is empty. "<span class="tex-font-style-tt">P</span>" means that this cell contains a little pig. "<span class="tex-font-style-tt">W</span>" means that this cell contains a wolf. </p><p>It is guaranteed that there will be at most one wolf adjacent to any little pig.</p></div><div class="output-specification"><p>Print a single number — the maximal number of little pigs that may be eaten by the wolves.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10</span>) which denotes the number of rows and columns in our two-dimensional grid, respectively. Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each — that is the grid description. "<span class="tex-font-style-tt">.</span>" means that this cell is empty. "<span class="tex-font-style-tt">P</span>" means that this cell contains a little pig. "<span class="tex-font-style-tt">W</span>" means that this cell contains a wolf. </p><p>It is guaranteed that there will be at most one wolf adjacent to any little pig.</p>

## Output

<p>Print a single number — the maximal number of little pigs that may be eaten by the wolves.</p>





```input1
2 3
PPW
W.P

```




```input2
3 3
P.W
.P.
W.P

```




```output1
2

```




```output2
0

```



## Note

<p>In the first example, one possible scenario in which two little pigs get eaten by the wolves is as follows. </p><center> <img class="tex-graphics" src="file://SScVSX8B.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
