## Description

<div><p>Omkar is creating a mosaic using colored square tiles, which he places in an $n \times n$ grid. When the mosaic is complete, each cell in the grid will have either a glaucous or sinoper tile. However, currently he has only placed tiles in some cells. </p><p>A completed mosaic will be a <span class="tex-font-style-bf">mastapeece</span> if and only if each tile is adjacent to exactly $2$ tiles of the same color ($2$ tiles are adjacent if they share a side.) Omkar wants to fill the rest of the tiles so that the mosaic becomes a <span class="tex-font-style-bf">mastapeece</span>. Now he is wondering, is the way to do this unique, and if it is, what is it?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 2000$).</p><p>Then follow $n$ lines with $n$ characters in each line. The $i$-th character in the $j$-th line corresponds to the cell in row $i$ and column $j$ of the grid, and will be $S$ if Omkar has placed a sinoper tile in this cell, $G$ if Omkar has placed a glaucous tile, $.$ if it's empty. </p></div><div class="output-specification"><p>On the first line, print <span class="tex-font-style-tt">UNIQUE</span> if there is a unique way to get a mastapeece, <span class="tex-font-style-tt">NONE</span> if Omkar cannot create any, and <span class="tex-font-style-tt">MULTIPLE</span> if there is more than one way to do so. <span class="tex-font-style-bf">All letters must be uppercase.</span></p><p>If you print <span class="tex-font-style-tt">UNIQUE</span>, then print $n$ additional lines with $n$ characters in each line, such that the $i$-th character in the $j^{\text{th}}$ line is $S$ if the tile in row $i$ and column $j$ of the mastapeece is sinoper, and $G$ if it is glaucous. </p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 2000$).</p><p>Then follow $n$ lines with $n$ characters in each line. The $i$-th character in the $j$-th line corresponds to the cell in row $i$ and column $j$ of the grid, and will be $S$ if Omkar has placed a sinoper tile in this cell, $G$ if Omkar has placed a glaucous tile, $.$ if it's empty. </p>

## Output

<p>On the first line, print <span class="tex-font-style-tt">UNIQUE</span> if there is a unique way to get a mastapeece, <span class="tex-font-style-tt">NONE</span> if Omkar cannot create any, and <span class="tex-font-style-tt">MULTIPLE</span> if there is more than one way to do so. <span class="tex-font-style-bf">All letters must be uppercase.</span></p><p>If you print <span class="tex-font-style-tt">UNIQUE</span>, then print $n$ additional lines with $n$ characters in each line, such that the $i$-th character in the $j^{\text{th}}$ line is $S$ if the tile in row $i$ and column $j$ of the mastapeece is sinoper, and $G$ if it is glaucous. </p>





```input1
4
S...
..G.
....
...S
```




```input2
6
S.....
....G.
..S...
.....S
....G.
G.....
```




```input3
10
.S....S...
..........
...SSS....
..........
..........
...GS.....
....G...G.
..........
......G...
..........
```




```input4
1
.
```




```output1
MULTIPLE
```




```output2
NONE
```




```output3
UNIQUE
SSSSSSSSSS
SGGGGGGGGS
SGSSSSSSGS
SGSGGGGSGS
SGSGSSGSGS
SGSGSSGSGS
SGSGGGGSGS
SGSSSSSSGS
SGGGGGGGGS
SSSSSSSSSS
```




```output4
NONE
```



## Note

<p>For the first test case, Omkar can make the mastapeeces</p><p><span class="tex-font-style-tt">SSSS</span></p><p><span class="tex-font-style-tt">SGGS</span></p><p><span class="tex-font-style-tt">SGGS</span></p><p><span class="tex-font-style-tt">SSSS</span></p><p>and </p><p><span class="tex-font-style-tt">SSGG</span></p><p><span class="tex-font-style-tt">SSGG</span></p><p><span class="tex-font-style-tt">GGSS</span></p><p><span class="tex-font-style-tt">GGSS</span>.</p><p>For the second test case, it can be proven that it is impossible for Omkar to add tiles to create a mastapeece.</p><p>For the third case, it can be proven that the given mastapeece is the only mastapeece Omkar can create by adding tiles.</p><p>For the fourth test case, it's clearly impossible for the only tile in any mosaic Omkar creates to be adjacent to two tiles of the same color, as it will be adjacent to $0$ tiles total. </p>
