## Description

<div><p>You have a garden consisting entirely of grass and weeds. Your garden is described by an <span class="tex-span"><i>n</i> × <i>m</i></span> grid, with rows numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom, and columns <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right. Each cell is identified by a pair <span class="tex-span">(<i>r</i>, <i>c</i>)</span> which means that the cell is located at row <span class="tex-span"><i>r</i></span> and column <span class="tex-span"><i>c</i></span>. Each cell may contain either grass or weeds. For example, a <span class="tex-span">4 × 5</span> garden may look as follows (empty cells denote grass):</p><center> <img class="tex-graphics" src="file://PwCKNPqr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You have a land-mower with you to mow all the weeds. Initially, you are standing with your lawnmower at the top-left corner of the garden. That is, at cell <span class="tex-span">(1, 1)</span>. At any moment of time you are facing a certain direction — either left or right. And initially, you face right.</p><p>In one move you can do either one of these:</p><p>1) Move one cell in the direction that you are facing.</p><ul><p> </p><li> if you are facing right: move from cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> to cell <span class="tex-span">(<i>r</i>, <i>c</i> + 1)</span><p> </p><center> <img class="tex-graphics" src="file://oGXfNhxU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p> </p></li><li> if you are facing left: move from cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> to cell <span class="tex-span">(<i>r</i>, <i>c</i> - 1)</span><p> </p><center> <img class="tex-graphics" src="file://MJ8rbo92.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li></ul> 2) Move one cell down (that is, from cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> to cell <span class="tex-span">(<i>r</i> + 1, <i>c</i>)</span>), and change your direction to the opposite one.<ul><p> </p><li> if you were facing right previously, you will face left<p> </p><center> <img class="tex-graphics" src="file://CwCBucjt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p> </p></li><li> if you were facing left previously, you will face right<p> </p><center> <img class="tex-graphics" src="file://Mvd0arzm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> </li></ul><p>You are not allowed to leave the garden. Weeds will be mowed if you and your lawnmower are standing at the cell containing the weeds (your direction doesn't matter). This action isn't counted as a move.</p><p>What is the minimum number of moves required to mow all the weeds?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 150</span>) — the number of rows and columns respectively. Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each — the content of the grid. "<span class="tex-font-style-tt">G</span>" means that this cell contains grass. "<span class="tex-font-style-tt">W</span>" means that this cell contains weeds. </p><p>It is guaranteed that the top-left corner of the grid will contain grass.</p></div><div class="output-specification"><p>Print a single number — the minimum number of moves required to mow all the weeds.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 150</span>) — the number of rows and columns respectively. Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each — the content of the grid. "<span class="tex-font-style-tt">G</span>" means that this cell contains grass. "<span class="tex-font-style-tt">W</span>" means that this cell contains weeds. </p><p>It is guaranteed that the top-left corner of the grid will contain grass.</p>

## Output

<p>Print a single number — the minimum number of moves required to mow all the weeds.</p>





```input1
4 5
GWGGW
GGWGG
GWGGG
WGGGG

```




```input2
3 3
GWW
WWW
WWG

```




```input3
1 1
G

```




```output1
11

```




```output2
7

```




```output3
0

```



## Note

<p>For the first example, this is the picture of the initial state of the grid:</p><center> <img class="tex-graphics" src="file://N6HUAeCs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A possible solution is by mowing the weeds as illustrated below:</p><center> <img class="tex-graphics" src="file://uA2CBRY0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
