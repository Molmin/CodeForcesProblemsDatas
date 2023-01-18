## Description

<div><p>Valera has got a rectangle table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Valera numbered the table rows starting from one, from top to bottom and the columns – starting from one, from left to right. We will represent cell that is on the intersection of row <span class="tex-span"><i>x</i></span> and column <span class="tex-span"><i>y</i></span> by a pair of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span>.</p><p>Valera wants to place exactly <span class="tex-span"><i>k</i></span> tubes on his rectangle table. A tube is such sequence of table cells <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">...</span>, <span class="tex-span">(<i>x</i><sub class="lower-index"><i>r</i></sub>, <i>y</i><sub class="lower-index"><i>r</i></sub>)</span>, that: </p><ul> <li> <span class="tex-span"><i>r</i> ≥ 2</span>; </li><li> for any integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>r</i> - 1)</span> the following equation <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i> + 1</sub>| + |<i>y</i><sub class="lower-index"><i>i</i></sub> - <i>y</i><sub class="lower-index"><i>i</i> + 1</sub>| = 1</span> holds; </li><li> each table cell, which belongs to the tube, must occur exactly once in the sequence. </li></ul><p>Valera thinks that the tubes are arranged in a fancy manner if the following conditions are fulfilled: </p><ul> <li> no pair of tubes has common cells; </li><li> each cell of the table belongs to some tube. </li></ul><p>Help Valera to arrange <span class="tex-span"><i>k</i></span> tubes on his rectangle table in a fancy manner.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 300</span>; <span class="tex-span">2 ≤ 2<i>k</i> ≤ <i>n</i>·<i>m</i></span>) — the number of rows, the number of columns and the number of tubes, correspondingly. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the description of the <span class="tex-span"><i>i</i></span>-th tube: first print integer <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (the number of tube cells), then print <span class="tex-span">2<i>r</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>1</sub>, <i>y</i><sub class="lower-index"><i>i</i>1</sub>, <i>x</i><sub class="lower-index"><i>i</i>2</sub>, <i>y</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>x</i><sub class="lower-index"><i>ir</i><sub class="lower-index"><i>i</i></sub></sub>, <i>y</i><sub class="lower-index"><i>ir</i><sub class="lower-index"><i>i</i></sub></sub></span> (the sequence of table cells).</p><p>If there are multiple solutions, you can print any of them. It is guaranteed that at least one solution exists. </p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 300</span>; <span class="tex-span">2 ≤ 2<i>k</i> ≤ <i>n</i>·<i>m</i></span>) — the number of rows, the number of columns and the number of tubes, correspondingly. </p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the description of the <span class="tex-span"><i>i</i></span>-th tube: first print integer <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (the number of tube cells), then print <span class="tex-span">2<i>r</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>1</sub>, <i>y</i><sub class="lower-index"><i>i</i>1</sub>, <i>x</i><sub class="lower-index"><i>i</i>2</sub>, <i>y</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>x</i><sub class="lower-index"><i>ir</i><sub class="lower-index"><i>i</i></sub></sub>, <i>y</i><sub class="lower-index"><i>ir</i><sub class="lower-index"><i>i</i></sub></sub></span> (the sequence of table cells).</p><p>If there are multiple solutions, you can print any of them. It is guaranteed that at least one solution exists. </p>





```input1
3 3 3

```




```input2
2 3 1

```




```output1
3 1 1 1 2 1 3
3 2 1 2 2 2 3
3 3 1 3 2 3 3

```




```output2
6 1 1 1 2 1 3 2 3 2 2 2 1

```



## Note

<p>Picture for the first sample: </p><center> <img class="tex-graphics" src="file://xPjS2CNx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Picture for the second sample: </p><center> <img class="tex-graphics" src="file://m5jYX93G.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
