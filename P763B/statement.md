## Description

<div><p>One of Timofey's birthday presents is a colourbook in a shape of an infinite plane. On the plane <span class="tex-span"><i>n</i></span> rectangles with sides parallel to coordinate axes are situated. All sides of the rectangles have <span class="tex-font-style-bf">odd</span> length. Rectangles cannot intersect, but they can touch each other.</p><p>Help Timofey to color his rectangles in <span class="tex-span">4</span> different colors in such a way that every two rectangles touching each other by side would have different color, or determine that it is impossible.</p><p>Two rectangles intersect if their intersection has positive area. Two rectangles touch by sides if there is a pair of sides such that their intersection has non-zero length</p><center> <img class="tex-graphics" height="272px" src="file://tWtMfeJC.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">The picture corresponds to the first example</span> </center></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rectangles.</p><p><span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of these lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>), that means that points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> are the coordinates of two opposite corners of the <span class="tex-span"><i>i</i></span>-th rectangle.</p><p>It is guaranteed, that all sides of the rectangles have <span class="tex-font-style-bf">odd</span> lengths and rectangles don't intersect each other.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" in the only line if it is impossible to color the rectangles in <span class="tex-span">4</span> different colors in such a way that every two rectangles touching each other by side would have different color.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line. Then print <span class="tex-span"><i>n</i></span> lines, in the <span class="tex-span"><i>i</i></span>-th of them print single integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>)&nbsp;— the color of <span class="tex-span"><i>i</i></span>-th rectangle.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rectangles.</p><p><span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of these lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>), that means that points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> are the coordinates of two opposite corners of the <span class="tex-span"><i>i</i></span>-th rectangle.</p><p>It is guaranteed, that all sides of the rectangles have <span class="tex-font-style-bf">odd</span> lengths and rectangles don't intersect each other.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" in the only line if it is impossible to color the rectangles in <span class="tex-span">4</span> different colors in such a way that every two rectangles touching each other by side would have different color.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line. Then print <span class="tex-span"><i>n</i></span> lines, in the <span class="tex-span"><i>i</i></span>-th of them print single integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>)&nbsp;— the color of <span class="tex-span"><i>i</i></span>-th rectangle.</p>





```input1
8
0 0 5 3
2 -1 5 0
-3 -4 2 -1
-1 -1 2 0
-3 0 0 5
5 2 10 3
7 -3 10 2
4 -2 7 -1

```




```output1
YES
1
2
2
3
2
2
4
1

```


