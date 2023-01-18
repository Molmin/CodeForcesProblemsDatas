## Description

<div><p>According to the legends the king of Berland Berl I was noted for his love of beauty and order. One day he ordered to tile the palace hall's floor where balls and receptions used to take place with black and white tiles according to a regular geometrical pattern invented by him. However, as is after the case, due to low financing there were only <span class="tex-span"><i>a</i></span> black and <span class="tex-span"><i>b</i></span> white tiles delivered to the palace. The other <span class="tex-span"><i>c</i></span> tiles were black and white (see the picture).</p><center> <img class="tex-graphics" src="file://A2tbF7uR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The initial plan failed! Having learned of that, the king gave a new command: tile the floor with the available tiles so that no black side of a tile touched a white one. The tiles are squares of one size <span class="tex-span">1 × 1</span>, every black and white tile can be rotated in one of the four ways. </p><p>The court programmer was given the task to work out the plan of tiling and he coped with the task and didn't suffer the consequences of disobedience. And can you cope with it?</p></div><div class="input-specification"><p>The first line contains given integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) which represent the sizes of the rectangle that needs to be tiled. The next line contains non-negative numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>a</i> + <i>b</i> + <i>c</i> = <i>nm</i></span>, <span class="tex-span"><i>c</i> ≥ <i>m</i></span>. </p></div><div class="output-specification"><p>Print <span class="tex-span">2<i>n</i></span> lines containing <span class="tex-span">2<i>m</i></span> characters each — the tiling scheme. Every tile is represented by a square <span class="tex-span">2 × 2</span> in the following manner (the order corresponds to the order of the picture above): </p><center> <img class="tex-graphics" src="file://7316nem7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> If multiple solutions exist, output any.</div>

## Input

<p>The first line contains given integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) which represent the sizes of the rectangle that needs to be tiled. The next line contains non-negative numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>a</i> + <i>b</i> + <i>c</i> = <i>nm</i></span>, <span class="tex-span"><i>c</i> ≥ <i>m</i></span>. </p>

## Output

<p>Print <span class="tex-span">2<i>n</i></span> lines containing <span class="tex-span">2<i>m</i></span> characters each — the tiling scheme. Every tile is represented by a square <span class="tex-span">2 × 2</span> in the following manner (the order corresponds to the order of the picture above): </p><center> <img class="tex-graphics" src="file://7316nem7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> If multiple solutions exist, output any.





```input1
2 2
0 0 4

```




```input2
2 3
1 2 3

```




```output1
<span class="tex-span">\</span>../
#<span class="tex-span">\</span>/#
<span class="tex-span">\</span>##/
.<span class="tex-span">\</span>/.

```




```output2
###/<span class="tex-span">\</span>#
##/..<span class="tex-span">\</span>
#/....
/.....

```


