## Description

<div><p>You might have heard about the next game in Lara Croft series coming out this year. You also might have watched its trailer. Though you definitely missed the main idea about its plot, so let me lift the veil of secrecy.</p><p>Lara is going to explore yet another dangerous dungeon. Game designers decided to use good old 2D environment. The dungeon can be represented as a rectangle matrix of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is the cell in the <span class="tex-span"><i>x</i></span>-th row in the <span class="tex-span"><i>y</i></span>-th column. Lara can move between the neighbouring by side cells in all four directions.</p><p>Moreover, she has even chosen the path for herself to avoid all the traps. She enters the dungeon in cell <span class="tex-span">(1, 1)</span>, that is top left corner of the matrix. Then she goes down all the way to cell <span class="tex-span">(<i>n</i>, 1)</span> — the bottom left corner. Then she starts moving in the snake fashion — all the way to the right, one cell up, then to the left to the cell in <span class="tex-span">2</span>-nd column, one cell up. She moves until she runs out of non-visited cells. <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> given are such that she always end up in cell <span class="tex-span">(1, 2)</span>.</p><p>Lara has already moved to a neighbouring cell <span class="tex-span"><i>k</i></span> times. Can you determine her current position?</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-font-style-bf"><span class="tex-span"><i>n</i></span> is always even</span>, <span class="tex-span">0 ≤ <i>k</i> &lt; <i>n</i>·<i>m</i></span>). Note that <span class="tex-span"><i>k</i></span> doesn't fit into <span class="tex-span">32</span>-bit integer type!</p></div><div class="output-specification"><p>Print the cell (the row and the column where the cell is situated) where Lara ends up after she moves <span class="tex-span"><i>k</i></span> times.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-font-style-bf"><span class="tex-span"><i>n</i></span> is always even</span>, <span class="tex-span">0 ≤ <i>k</i> &lt; <i>n</i>·<i>m</i></span>). Note that <span class="tex-span"><i>k</i></span> doesn't fit into <span class="tex-span">32</span>-bit integer type!</p>

## Output

<p>Print the cell (the row and the column where the cell is situated) where Lara ends up after she moves <span class="tex-span"><i>k</i></span> times.</p>





```input1
4 3 0

```




```input2
4 3 11

```




```input3
4 3 7

```




```output1
1 1

```




```output2
1 2

```




```output3
3 2

```



## Note

<p>Here is her path on matrix <span class="tex-span">4</span> by <span class="tex-span">3</span>:</p><center> <img class="tex-graphics" src="file://jawpvnoC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
