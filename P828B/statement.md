## Description

<div><p>Polycarp has a checkered sheet of paper of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Polycarp painted some of cells with black, the others remained white. Inspired by Malevich's "Black Square", Polycarp wants to paint minimum possible number of white cells with black so that all black cells form a square.</p><p>You are to determine the minimum possible number of cells needed to be painted black so that the black cells form a black square with sides parallel to the painting's sides. All the cells that do not belong to the square should be white. The square's side should have positive length.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the sizes of the sheet.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> letters '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>' each — the description of initial cells' colors. If a letter is '<span class="tex-font-style-tt">B</span>', then the corresponding cell is painted black, otherwise it is painted white.</p></div><div class="output-specification"><p>Print the minimum number of cells needed to be painted black so that the black cells form a black square with sides parallel to the painting's sides. All the cells that do not belong to the square should be white. If it is impossible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the sizes of the sheet.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> letters '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>' each — the description of initial cells' colors. If a letter is '<span class="tex-font-style-tt">B</span>', then the corresponding cell is painted black, otherwise it is painted white.</p>

## Output

<p>Print the minimum number of cells needed to be painted black so that the black cells form a black square with sides parallel to the painting's sides. All the cells that do not belong to the square should be white. If it is impossible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 4
WWWW
WWWB
WWWB
WWBB
WWWW

```




```input2
1 2
BB

```




```input3
3 3
WWW
WWW
WWW

```




```output1
5

```




```output2
-1

```




```output3
1

```



## Note

<p>In the first example it is needed to paint <span class="tex-span">5</span> cells — <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(3, 2)</span>, <span class="tex-span">(3, 3)</span> and <span class="tex-span">(4, 2)</span>. Then there will be a square with side equal to three, and the upper left corner in <span class="tex-span">(2, 2)</span>.</p><p>In the second example all the cells are painted black and form a rectangle, so it's impossible to get a square.</p><p>In the third example all cells are colored white, so it's sufficient to color any cell black.</p>
