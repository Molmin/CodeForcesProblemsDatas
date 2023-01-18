## Description

<div><p>Little John aspires to become a plumber! Today he has drawn a grid consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns, consisting of <span class="tex-span"><i>n</i> × <i>m</i></span> square cells.</p><p>In each cell he will draw a pipe segment. He can only draw four types of segments numbered from <span class="tex-span">1</span> to <span class="tex-span">4</span>, illustrated as follows:</p><center> <img class="tex-graphics" src="file://dTCceuKr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Each pipe segment has two ends, illustrated by the arrows in the picture above. For example, segment <span class="tex-span">1</span> has ends at top and left side of it.</p><p>Little John considers the piping system to be leaking if there is at least one pipe segment inside the grid whose end is not connected to another pipe's end or to the border of the grid. The image below shows an example of leaking and non-leaking systems of size <span class="tex-span">1 × 2</span>.</p><center> <img class="tex-graphics" src="file://qhZH2Ykl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now, you will be given the grid that has been partially filled by Little John. Each cell will either contain one of the four segments above, or be empty. Find the number of possible different non-leaking final systems after Little John finishes filling <span class="tex-font-style-bf">all</span> of the empty cells with pipe segments. Print this number modulo <span class="tex-span">1000003</span> (<span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>).</p><p>Note that rotations or flipping of the grid are not allowed and so two configurations that are identical only when one of them has been rotated or flipped either horizontally or vertically are considered two different configurations.</p></div><div class="input-specification"><p>The first line will contain two single-space separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>n</i>·<i>m</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of rows and columns respectively. Then <span class="tex-span"><i>n</i></span> lines follow, each contains exactly <span class="tex-span"><i>m</i></span> characters — the description of the grid. Each character describes a cell and is either one of these: </p><ul> <li> "<span class="tex-font-style-tt">1</span>" - "<span class="tex-font-style-tt">4</span>" — a pipe segment of one of four types as described above </li><li> "<span class="tex-font-style-tt">.</span>" — an empty cell </li></ul></div><div class="output-specification"><p>Print a single integer denoting the number of possible final non-leaking pipe systems modulo <span class="tex-span">1000003</span> (<span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>). If there are no such configurations, print <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line will contain two single-space separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>n</i>·<i>m</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of rows and columns respectively. Then <span class="tex-span"><i>n</i></span> lines follow, each contains exactly <span class="tex-span"><i>m</i></span> characters — the description of the grid. Each character describes a cell and is either one of these: </p><ul> <li> "<span class="tex-font-style-tt">1</span>" - "<span class="tex-font-style-tt">4</span>" — a pipe segment of one of four types as described above </li><li> "<span class="tex-font-style-tt">.</span>" — an empty cell </li></ul>

## Output

<p>Print a single integer denoting the number of possible final non-leaking pipe systems modulo <span class="tex-span">1000003</span> (<span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>). If there are no such configurations, print <span class="tex-span">0</span>.</p>





```input1
2 2
13
..

```




```input2
3 1
1
4
.

```




```input3
2 2
3.
.1

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>For the first example, the initial configuration of the grid is as follows. </p><center> <img class="tex-graphics" src="file://Q2GQ4kFo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The only two possible final non-leaking pipe configurations are as follows:</p><center> <img class="tex-graphics" src="file://fljCCCDu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://YzhafceS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second example, the initial grid is already leaking, so there will be no final grid that is non-leaking.</p><p>For the final example, there's only one possible non-leaking final grid as follows.</p><center> <img class="tex-graphics" src="file://9OXwq8yb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
