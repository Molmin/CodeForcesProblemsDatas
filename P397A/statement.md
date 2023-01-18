## Description

<div><p>Our old friend Alexey has finally entered the University of City N — the Berland capital. Alexey expected his father to get him a place to live in but his father said it was high time for Alexey to practice some financial independence. So, Alexey is living in a dorm. </p><p>The dorm has exactly one straight dryer — a <span class="tex-span">100</span> centimeter long rope to hang clothes on. The dryer has got a coordinate system installed: the leftmost end of the dryer has coordinate <span class="tex-span">0</span>, and the opposite end has coordinate <span class="tex-span">100</span>. Overall, the university has <span class="tex-span"><i>n</i></span> students. Dean's office allows <span class="tex-span"><i>i</i></span>-th student to use the segment <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> of the dryer. However, the dean's office actions are contradictory and now one part of the dryer can belong to multiple students!</p><p>Alexey don't like when someone touch his clothes. That's why he want make it impossible to someone clothes touch his ones. So Alexey wonders: what is the total length of the parts of the dryer that he may use in a such way that clothes of the others <span class="tex-span">(<i>n</i> - 1)</span> students aren't drying there. Help him! Note that Alexey, as the most respected student, has number 1.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The <span class="tex-span">(<i>i</i> + 1)</span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) —&nbsp;the endpoints of the corresponding segment for the <span class="tex-span"><i>i</i></span>-th student.</p></div><div class="output-specification"><p>On a single line print a single number <span class="tex-span"><i>k</i></span>, equal to the sum of lengths of the parts of the dryer which are inside Alexey's segment and are outside all other segments.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The <span class="tex-span">(<i>i</i> + 1)</span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) —&nbsp;the endpoints of the corresponding segment for the <span class="tex-span"><i>i</i></span>-th student.</p>

## Output

<p>On a single line print a single number <span class="tex-span"><i>k</i></span>, equal to the sum of lengths of the parts of the dryer which are inside Alexey's segment and are outside all other segments.</p>





```input1
3
0 5
2 8
1 6

```




```input2
3
0 10
1 5
7 15

```




```output1
1

```




```output2
3

```



## Note

<p>Note that it's not important are clothes drying on the touching segments (e.g. <span class="tex-span">(0, 1)</span> and <span class="tex-span">(1, 2)</span>) considered to be touching or not because you need to find the length of segments.</p><p>In the first test sample Alexey may use the only segment <span class="tex-span">(0, 1)</span>. In such case his clothes will not touch clothes on the segments <span class="tex-span">(1, 6)</span> and <span class="tex-span">(2, 8)</span>. The length of segment <span class="tex-span">(0, 1)</span> is 1.</p><p>In the second test sample Alexey may dry his clothes on segments <span class="tex-span">(0, 1)</span> and <span class="tex-span">(5, 7)</span>. Overall length of these segments is 3.</p>
