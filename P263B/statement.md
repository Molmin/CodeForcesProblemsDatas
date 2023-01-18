## Description

<div><p>Vasya has found a piece of paper with a coordinate system written on it. There are <span class="tex-span"><i>n</i></span> distinct squares drawn in this coordinate system. Let's number the squares with integers from 1 to <span class="tex-span"><i>n</i></span>. It turned out that points with coordinates <span class="tex-span">(0, 0)</span> and <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>)</span> are the opposite corners of the <span class="tex-span"><i>i</i></span>-th square.</p><p>Vasya wants to find such integer point (with integer coordinates) of the plane, that belongs to exactly <span class="tex-span"><i>k</i></span> drawn squares. We'll say that a point belongs to a square, if the point is located either inside the square, or on its boundary. </p><p>Help Vasya find a point that would meet the described limits.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 50)</span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that all given squares are distinct.</p></div><div class="output-specification"><p>In a single line print two space-separated integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of the point that belongs to exactly <span class="tex-span"><i>k</i></span> squares. If there are multiple answers, you are allowed to print any of them. </p><p>If there is no answer, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 50)</span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that all given squares are distinct.</p>

## Output

<p>In a single line print two space-separated integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of the point that belongs to exactly <span class="tex-span"><i>k</i></span> squares. If there are multiple answers, you are allowed to print any of them. </p><p>If there is no answer, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p>





```input1
4 3
5 1 3 4

```




```input2
3 1
2 4 1

```




```input3
4 50
5 1 10 2

```




```output1
2 1

```




```output2
4 0

```




```output3
-1

```


