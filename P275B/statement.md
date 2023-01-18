## Description

<div><p>Consider an <span class="tex-span"><i>n</i> × <i>m</i></span> grid. Initially all the cells of the grid are colored white. Lenny has painted some of the cells (at least one) black. We call a painted grid <span class="tex-font-style-underline">convex</span> if one can walk from <span class="tex-font-style-bf">any</span> black cell to <span class="tex-font-style-bf">any another</span> black cell using a path of side-adjacent black cells changing his direction at most once during the path. In the figure below, the left grid is convex while the right one is not convex, because there exist two cells which need more than one time to change direction in their path.</p><center> <img class="tex-graphics" src="file://6XU7L2fO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You're given a painted grid in the input. Tell Lenny if the grid is convex or not.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 50)</span> — the size of the grid. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">B</span>" or "<span class="tex-font-style-tt">W</span>". Character "<span class="tex-font-style-tt">B</span>" denotes a black cell of the grid and "<span class="tex-font-style-tt">W</span>" denotes a white cell of the grid.</p><p>It's guaranteed that the grid has at least one black cell.</p></div><div class="output-specification"><p>On the only line of the output print "<span class="tex-font-style-tt">YES</span>" if the grid is convex, otherwise print "<span class="tex-font-style-tt">NO</span>". Do not print quotes.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 50)</span> — the size of the grid. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">B</span>" or "<span class="tex-font-style-tt">W</span>". Character "<span class="tex-font-style-tt">B</span>" denotes a black cell of the grid and "<span class="tex-font-style-tt">W</span>" denotes a white cell of the grid.</p><p>It's guaranteed that the grid has at least one black cell.</p>

## Output

<p>On the only line of the output print "<span class="tex-font-style-tt">YES</span>" if the grid is convex, otherwise print "<span class="tex-font-style-tt">NO</span>". Do not print quotes.</p>





```input1
3 4
WWBW
BWWW
WWWB

```




```input2
3 1
B
B
W

```




```output1
NO

```




```output2
YES

```


