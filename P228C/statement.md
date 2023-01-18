## Description

<div><p>Little Vasya likes painting fractals very much.</p><p>He does it like this. First the boy cuts out a <span class="tex-span">2 × 2</span>-cell square out of squared paper. Then he paints some cells black. The boy calls the cut out square a fractal <span class="tex-font-style-it">pattern</span>. Then he takes a clean square sheet of paper and paints a fractal by the following algorithm:</p><ol> <li> He divides the sheet into four identical squares. A part of them is painted black according to the fractal pattern. </li><li> Each square that remained white, is split into 4 lesser white squares, some of them are painted according to the fractal pattern. Each square that remained black, is split into 4 lesser black squares. </li></ol> <p>In each of the following steps step 2 repeats. To draw a fractal, the boy can make an arbitrary positive number of steps of the algorithm. But he need to make at least two steps. In other words step 2 of the algorithm <span class="tex-font-style-bf">must be done at least once</span>. The resulting picture (the square with painted cells) will be a fractal. The figure below shows drawing a fractal (here boy made three steps of the algorithm).</p><center> <img class="tex-graphics" src="file://xFZKeUQk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>One evening Vasya got very tired, so he didn't paint the fractal, he just took a sheet of paper, painted a <span class="tex-span"><i>n</i> × <i>m</i></span>-cell field. Then Vasya paint some cells black. </p><p>Now he wonders, how many squares are on the field, such that there is a fractal, which can be obtained as described above, and which is equal to that square. Square is considered equal to some fractal if they consist of the same amount of elementary not divided cells and for each elementary cell of the square corresponding elementary cell of the fractal have the same color.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 500)</span> — the number of rows and columns of the field, correspondingly. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the description of the field, painted by Vasya. Character "<span class="tex-font-style-tt">.</span>" represents a white cell, character "<span class="tex-font-style-tt">*</span>" represents a black cell.</p><p>It is guaranteed that the field description doesn't contain other characters than "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>".</p></div><div class="output-specification"><p>On a single line print a single integer — the number of squares on the field, such that these squares contain a drawn fractal, which can be obtained as described above.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 500)</span> — the number of rows and columns of the field, correspondingly. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the description of the field, painted by Vasya. Character "<span class="tex-font-style-tt">.</span>" represents a white cell, character "<span class="tex-font-style-tt">*</span>" represents a black cell.</p><p>It is guaranteed that the field description doesn't contain other characters than "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>".</p>

## Output

<p>On a single line print a single integer — the number of squares on the field, such that these squares contain a drawn fractal, which can be obtained as described above.</p>





```input1
6 11
......*.***
*.*.*....**
.***....*.*
..***.*....
.*.*.....**
......*.*..

```




```input2
4 4
..**
..**
....
....

```




```output1
3

```




```output2
0

```



## Note

<p>The answer for the first sample is shown on the picture below. Fractals are outlined by red, blue and green squares.</p><center> <img class="tex-graphics" src="file://URzwZhYN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The answer for the second sample is 0. There is no fractal, equal to the given picture.</p><center> <img class="tex-graphics" src="file://rdra31qE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
