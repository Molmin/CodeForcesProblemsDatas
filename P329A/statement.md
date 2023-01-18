## Description

<div><p>You are an adventurer currently journeying inside an evil temple. After defeating a couple of weak zombies, you arrived at a square room consisting of tiles forming an <span class="tex-span"><i>n</i> × <i>n</i></span> grid. The rows are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> from top to bottom, and the columns are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> from left to right. At the far side of the room lies a door locked with evil magical forces. The following inscriptions are written on the door:</p><center> <span class="tex-font-style-underline">The cleaning of all evil will awaken the door!</span> </center><p>Being a very senior adventurer, you immediately realize what this means. You notice that every single cell in the grid are initially evil. You should purify all of these cells.</p><p>The only method of tile purification known to you is by casting the "Purification" spell. You cast this spell on a single tile — then, all cells that are located in the same row and all cells that are located in the same column as the selected tile become purified (including the selected tile)! It is allowed to purify a cell more than once.</p><p>You would like to purify all <span class="tex-span"><i>n</i> × <i>n</i></span> cells while minimizing the number of times you cast the "Purification" spell. This sounds very easy, but you just noticed that some tiles are particularly more evil than the other tiles. You cannot cast the "Purification" spell on those particularly more evil tiles, not even after they have been purified. They can still be purified if a cell sharing the same row or the same column gets selected by the "Purification" spell.</p><p>Please find some way to purify all the cells with the minimum number of spells cast. Print -1 if there is no such way.</p></div><div class="input-specification"><p>The first line will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then, <span class="tex-span"><i>n</i></span> lines follows, each contains <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th row represents the cell located at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span>. It will be the character '<span class="tex-font-style-tt">E</span>' if it is a particularly more evil cell, and '<span class="tex-font-style-tt">.</span>' otherwise.</p></div><div class="output-specification"><p>If there exists no way to purify all the cells, output -1. Otherwise, if your solution casts <span class="tex-span"><i>x</i></span> "Purification" spells (where <span class="tex-span"><i>x</i></span> is the minimum possible number of spells), output <span class="tex-span"><i>x</i></span> lines. Each line should consist of two integers denoting the row and column numbers of the cell on which you should cast the "Purification" spell.</p></div>

## Input

<p>The first line will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Then, <span class="tex-span"><i>n</i></span> lines follows, each contains <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th row represents the cell located at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span>. It will be the character '<span class="tex-font-style-tt">E</span>' if it is a particularly more evil cell, and '<span class="tex-font-style-tt">.</span>' otherwise.</p>

## Output

<p>If there exists no way to purify all the cells, output -1. Otherwise, if your solution casts <span class="tex-span"><i>x</i></span> "Purification" spells (where <span class="tex-span"><i>x</i></span> is the minimum possible number of spells), output <span class="tex-span"><i>x</i></span> lines. Each line should consist of two integers denoting the row and column numbers of the cell on which you should cast the "Purification" spell.</p>





```input1
3
.E.
E.E
.E.

```




```input2
3
EEE
E..
E.E

```




```input3
5
EE.EE
E.EE.
E...E
.EE.E
EE.EE

```




```output1
1 1
2 2
3 3

```




```output2
-1

```




```output3
3 3
1 3
2 2
4 4
5 3
```



## Note

<p>The first example is illustrated as follows. Purple tiles are evil tiles that have not yet been purified. Red tile is the tile on which "Purification" is cast. Yellow tiles are the tiles being purified as a result of the current "Purification" spell. Green tiles are tiles that have been purified previously. </p><center> <img class="tex-graphics" src="file://nMaPnWNU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, it is impossible to purify the cell located at row <span class="tex-span">1</span> and column <span class="tex-span">1</span>.</p><p>For the third example:</p><center> <img class="tex-graphics" src="file://PwDPhQnW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
