## Description

<div><p>One day Alice was cleaning up her basement when she noticed something very curious: an <span class="tex-font-style-bf">infinite</span> set of wooden pieces! Each piece was made of five square tiles, with four tiles adjacent to the fifth center tile: </p><center> <img class="tex-graphics" src="file://MF06QBIi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> By the pieces lay a large square wooden board. The board is divided into $n^2$ cells arranged into $n$ rows and $n$ columns. Some of the cells are already occupied by single tiles stuck to it. The remaining cells are free.<p>Alice started wondering whether she could fill the board completely using the pieces she had found. Of course, each piece has to cover exactly five distinct cells of the board, no two pieces can overlap and every piece should fit in the board entirely, without some parts laying outside the board borders. The board however was too large for Alice to do the tiling by hand. Can you help determine if it's possible to fully tile the board?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($3 \leq n \leq 50$) — the size of the board.</p><p>The following $n$ lines describe the board. The $i$-th line ($1 \leq i \leq n$) contains a single string of length $n$. Its $j$-th character ($1 \leq j \leq n$) is equal to "<span class="tex-font-style-tt">.</span>" if the cell in the $i$-th row and the $j$-th column is free; it is equal to "<span class="tex-font-style-tt">#</span>" if it's occupied.</p><p>You can assume that the board contains at least one free cell.</p></div><div class="output-specification"><p>Output <span class="tex-font-style-tt">YES</span> if the board can be tiled by Alice's pieces, or <span class="tex-font-style-tt">NO</span> otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($3 \leq n \leq 50$) — the size of the board.</p><p>The following $n$ lines describe the board. The $i$-th line ($1 \leq i \leq n$) contains a single string of length $n$. Its $j$-th character ($1 \leq j \leq n$) is equal to "<span class="tex-font-style-tt">.</span>" if the cell in the $i$-th row and the $j$-th column is free; it is equal to "<span class="tex-font-style-tt">#</span>" if it's occupied.</p><p>You can assume that the board contains at least one free cell.</p>

## Output

<p>Output <span class="tex-font-style-tt">YES</span> if the board can be tiled by Alice's pieces, or <span class="tex-font-style-tt">NO</span> otherwise. You can print each letter in any case (upper or lower).</p>





```input1
3
#.#
...
#.#
```




```input2
4
##.#
#...
####
##.#
```




```input3
5
#.###
....#
#....
###.#
#####
```




```input4
5
#.###
....#
#....
....#
#..##
```




```output1
YES
```




```output2
NO
```




```output3
YES
```




```output4
NO
```



## Note

<p>The following sketches show the example boards and their tilings if such tilings exist: </p><center> <img class="tex-graphics" src="file://tdsVpXG7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
