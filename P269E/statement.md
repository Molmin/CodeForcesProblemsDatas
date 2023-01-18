## Description

<div><p>Emuskald is an innovative musician and always tries to push the boundaries of music production. Now he has come up with an idea for a revolutionary musical instrument — a rectangular harp.</p><p>A rectangular harp is a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span> consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. The rows are numbered 1 to <span class="tex-span"><i>n</i></span> from top to bottom. Similarly the columns are numbered 1 to <span class="tex-span"><i>m</i></span> from left to right. String pins are spaced evenly across every side, one per unit. Thus there are <span class="tex-span"><i>n</i></span> pins on the left and right sides of the harp and <span class="tex-span"><i>m</i></span> pins on its top and bottom. The harp has exactly <span class="tex-span"><i>n</i> + <i>m</i></span> different strings, each string connecting two different pins, each on a different side of the harp.</p><p>Emuskald has ordered his apprentice to construct the first ever rectangular harp. However, he didn't mention that no two strings can cross, otherwise it would be impossible to play the harp. Two strings cross if the segments connecting their pins intersect. To fix the harp, Emuskald can perform operations of two types: </p><ol> <li> pick two different columns and swap their pins on each side of the harp, not changing the pins that connect each string; </li><li> pick two different rows and swap their pins on each side of the harp, not changing the pins that connect each string; </li></ol><p>In the following example, he can fix the harp by swapping two columns: </p><center> <img class="tex-graphics" src="file://MMQH3UVw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help Emuskald complete his creation and find the permutations how the rows and columns of the harp need to be rearranged, or tell that it is impossible to do so. He can detach and reattach each string to its pins, so the physical layout of the strings doesn't matter.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the height and width of the harp in units. Each of the following <span class="tex-span"><i>n</i> + <i>m</i></span> lines contains 4 space-separated tokens, describing a single string: two symbols <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and two integer numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. The pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> describes the first pin, and the pair <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> describes the second pin of the string;</p><p>A pair <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>x</i></span> describes the position of a single pin in a following way: </p><ol> <li> <span class="tex-span"><i>s</i></span> is equal to one of the symbols "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">R</span>" or "<span class="tex-font-style-tt">B</span>" (without quotes), which means that the pin is positioned on the left, top, right or bottom side of the harp accordingly; </li><li> <span class="tex-span"><i>x</i></span> is equal to the number of the row, if the pin is on the left or right border of the harp, and to the number of the column, if the pin is on the top or bottom border of the harp. </li></ol><p>It is guaranteed that no two different strings are connected to the same pin.</p></div><div class="output-specification"><p>If it is possible to rearrange the rows and columns to fix the harp, on the first line output <span class="tex-span"><i>n</i></span> space-separated integers — the old numbers of rows now placed from top to bottom in the fixed harp. On the second line, output <span class="tex-span"><i>m</i></span> space-separated integers — the old numbers of columns now placed from left to right in the fixed harp.</p><p>If it is impossible to rearrange the rows and columns to fix the harp, output "<span class="tex-font-style-tt">No solution</span>" (without quotes).</p></div>

## Input

<p>The first line of input contains two space-separated integers numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the height and width of the harp in units. Each of the following <span class="tex-span"><i>n</i> + <i>m</i></span> lines contains 4 space-separated tokens, describing a single string: two symbols <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and two integer numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. The pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> describes the first pin, and the pair <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> describes the second pin of the string;</p><p>A pair <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>x</i></span> describes the position of a single pin in a following way: </p><ol> <li> <span class="tex-span"><i>s</i></span> is equal to one of the symbols "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">R</span>" or "<span class="tex-font-style-tt">B</span>" (without quotes), which means that the pin is positioned on the left, top, right or bottom side of the harp accordingly; </li><li> <span class="tex-span"><i>x</i></span> is equal to the number of the row, if the pin is on the left or right border of the harp, and to the number of the column, if the pin is on the top or bottom border of the harp. </li></ol><p>It is guaranteed that no two different strings are connected to the same pin.</p>

## Output

<p>If it is possible to rearrange the rows and columns to fix the harp, on the first line output <span class="tex-span"><i>n</i></span> space-separated integers — the old numbers of rows now placed from top to bottom in the fixed harp. On the second line, output <span class="tex-span"><i>m</i></span> space-separated integers — the old numbers of columns now placed from left to right in the fixed harp.</p><p>If it is impossible to rearrange the rows and columns to fix the harp, output "<span class="tex-font-style-tt">No solution</span>" (without quotes).</p>





```input1
3 4
L T 1 3
L B 2 2
L B 3 3
T R 1 2
T B 2 1
T R 4 1
B R 4 3

```




```input2
3 3
L T 1 1
T R 3 1
R B 3 3
B L 1 3
L R 2 2
T B 2 2

```




```output1
1 2 3 
3 2 1 4 

```




```output2
No solution

```


