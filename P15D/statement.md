## Description

<div><p>There is an area map that is a rectangular matrix <span class="tex-span"><i>n</i> × <i>m</i></span>, each cell of the matrix contains the average height of a corresponding area part. Peter works for a company that has to build several cities within this area, each of the cities will occupy a rectangle <span class="tex-span"><i>a</i> × <i>b</i></span> cells on the map. To start construction works in a particular place Peter needs to remove excess ground from the construction site where a new city will be built. To do so he chooses a cell of the minimum height within this site, and removes excess ground from other cells of the site down to this minimum level. Let's consider that to lower the ground level from <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> to <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> (<span class="tex-span"><i>h</i><sub class="lower-index">1</sub> ≤ <i>h</i><sub class="lower-index">2</sub></span>) they need to remove <span class="tex-span"><i>h</i><sub class="lower-index">2</sub> - <i>h</i><sub class="lower-index">1</sub></span> ground units.</p><p>Let's call a site's position optimal, if the amount of the ground removed from this site is minimal compared to other possible positions. Peter constructs cities according to the following algorithm: from all the optimum site's positions he chooses the uppermost one. If this position is not unique, he chooses the leftmost one. Then he builds a city on this site. Peter repeats this process untill he can build at least one more city. For sure, he cannot carry out construction works on the occupied cells. Would you, please, help Peter place cities according to the algorithm? </p></div><div class="input-specification"><p>The first line contains four space-separated integers: map sizes <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and city sizes <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ <i>m</i> ≤ 1000</span>). Then there follow <span class="tex-span"><i>n</i></span> lines, each contains <span class="tex-span"><i>m</i></span> non-negative space-separated numbers, describing the height matrix. Each number doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. </p></div><div class="output-specification"><p>In the first line output <span class="tex-span"><i>k</i></span> — the amount of constructed cities. In each of the following <span class="tex-span"><i>k</i></span> lines output 3 space-separated numbers — the row number and the column number of the upper-left corner of a subsequent construction site, and the amount of the ground to remove from it. Output the sites in the order of their building up.</p></div>

## Input

<p>The first line contains four space-separated integers: map sizes <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and city sizes <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ <i>m</i> ≤ 1000</span>). Then there follow <span class="tex-span"><i>n</i></span> lines, each contains <span class="tex-span"><i>m</i></span> non-negative space-separated numbers, describing the height matrix. Each number doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. </p>

## Output

<p>In the first line output <span class="tex-span"><i>k</i></span> — the amount of constructed cities. In each of the following <span class="tex-span"><i>k</i></span> lines output 3 space-separated numbers — the row number and the column number of the upper-left corner of a subsequent construction site, and the amount of the ground to remove from it. Output the sites in the order of their building up.</p>





```input1
2 2 1 2
1 2
3 5

```




```input2
4 4 2 2
1 5 3 4
2 7 6 1
1 1 2 2
2 2 1 2

```




```output1
2
1 1 1
2 1 2

```




```output2
3
3 1 2
3 3 3
1 2 9

```


