## Description

<div><p><span class="tex-font-style-it">Connect the countless points with lines, till we reach the faraway yonder.</span></p><p>There are <span class="tex-span"><i>n</i></span> points on a coordinate plane, the <span class="tex-span"><i>i</i></span>-th of which being <span class="tex-span">(<i>i</i>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>Determine whether it's possible to draw two parallel and non-overlapping lines, such that every point in the set lies on <span class="tex-font-style-bf">exactly one</span> of them, and each of them passes through <span class="tex-font-style-bf">at least one</span> point in the set.</p></div><div class="input-specification"><p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1 000</span>) — the number of points.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the vertical coordinates of each point.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it's possible to fulfill the requirements, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1 000</span>) — the number of points.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the vertical coordinates of each point.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it's possible to fulfill the requirements, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
5
7 5 8 6 9

```




```input2
5
-1 -2 0 0 -5

```




```input3
5
5 4 3 2 1

```




```input4
5
1000000000 0 0 0 0

```




```output1
Yes

```




```output2
No

```




```output3
No

```




```output4
Yes

```



## Note

<p>In the first example, there are five points: <span class="tex-span">(1, 7)</span>, <span class="tex-span">(2, 5)</span>, <span class="tex-span">(3, 8)</span>, <span class="tex-span">(4, 6)</span> and <span class="tex-span">(5, 9)</span>. It's possible to draw a line that passes through points <span class="tex-span">1, 3, 5</span>, and another one that passes through points <span class="tex-span">2, 4</span> and is parallel to the first one.</p><p>In the second example, while it's possible to draw two lines that cover all points, they cannot be made parallel.</p><p>In the third example, it's impossible to satisfy both requirements at the same time.</p>
