## Description

<div><p>Emperor Palpatine loves owls very much. The emperor has some blueprints with the new Death Star, the blueprints contain <span class="tex-span"><i>n</i></span> distinct segments and <span class="tex-span"><i>m</i></span> distinct circles. We will consider the segments indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some way and the circles — indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in some way. </p><p>Palpatine defines an owl as a set of a pair of distinct circles <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) and one segment <span class="tex-span"><i>k</i></span>, such that: </p><ol> <li> circles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are symmetrical relatively to the straight line containing segment <span class="tex-span"><i>k</i></span>; </li><li> circles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> don't have any common points; </li><li> circles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> have the same radius; </li><li> segment <span class="tex-span"><i>k</i></span> intersects the segment that connects the centers of circles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. </li></ol><p>Help Palpatine, count the number of distinct owls on the picture. </p></div><div class="input-specification"><p>The first line contains two integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 1500</span>). </p><p>The next <span class="tex-span"><i>n</i></span> lines contain four integers each, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the coordinates of the two endpoints of the segment. It's guaranteed that each segment has positive length.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain three integers each, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the center and the radius of the <span class="tex-span"><i>i</i></span>-th circle. All coordinates are integers of at most <span class="tex-span">10<sup class="upper-index">4</sup></span> in their absolute value. The radius is a positive integer of at most <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p><p>It is guaranteed that all segments and all circles are dictinct.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to output 64-bit integers is С++. It is preferred to use the <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 1500</span>). </p><p>The next <span class="tex-span"><i>n</i></span> lines contain four integers each, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the coordinates of the two endpoints of the segment. It's guaranteed that each segment has positive length.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain three integers each, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the center and the radius of the <span class="tex-span"><i>i</i></span>-th circle. All coordinates are integers of at most <span class="tex-span">10<sup class="upper-index">4</sup></span> in their absolute value. The radius is a positive integer of at most <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p><p>It is guaranteed that all segments and all circles are dictinct.</p>

## Output

<p>Print a single number — the answer to the problem.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to output 64-bit integers is С++. It is preferred to use the <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1 2
3 2 3 -2
0 0 2
6 0 2

```




```input2
3 2
0 0 0 1
0 -1 0 1
0 -1 0 0
2 0 1
-2 0 1

```




```input3
1 2
-1 0 1 0
-100 0 1
100 0 1

```




```output1
1

```




```output2
3

```




```output3
0

```



## Note

<p>Here's an owl from the first sample. The owl is sitting and waiting for you to count it. </p><center> <img class="tex-graphics" src="file://6GncjLQe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
