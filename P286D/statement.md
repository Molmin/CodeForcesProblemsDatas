## Description

<div><p>A double tourist path, located at a park in Ultima Thule, is working by the following principle:</p><ul> <li> We introduce the Cartesian coordinate system. </li><li> At some points of time there are two tourists going (for a walk) from points <span class="tex-span">( - 1, 0)</span> and <span class="tex-span">(1, 0)</span> simultaneously. The first one is walking from <span class="tex-span">( - 1, 0)</span>, the second one is walking from <span class="tex-span">(1, 0)</span>. </li><li> Both tourists in a pair move at the same speed <span class="tex-span">1</span> (distance unit per second), the first one moves along line <span class="tex-span"><i>x</i> =  - 1</span>, the second one moves along line <span class="tex-span"><i>x</i> = 1</span>, both of them are moving in the positive direction of the <span class="tex-span"><i>Oy</i></span> axis. </li><li> At some points of time walls appear. Wall <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> is a segment between points <span class="tex-span">(0, <i>l</i><sub class="lower-index"><i>i</i></sub>)</span> and <span class="tex-span">(0, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span>. Each wall appears immediately. </li></ul><p>The Ultima Thule government wants to learn this for each pair of tourists that walk simultaneously: for how long (in seconds) will they not see each other? Two tourists don't see each other if the segment that connects their positions on the plane intersects at least one wall. Two segments intersect if they share at least one point. We assume that the segments' ends belong to the segments.</p><p>Help the government count the required time. Note that the walls can intersect (in any way) or coincide.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs of tourists and the number of built walls. The next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> each (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the wall ends and the time it appeared. The last line contains <span class="tex-span"><i>n</i></span> distinct space-separated strictly increasing integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the points of time when pairs of tourists walk.</p><p>All points of time are given in seconds.</p></div><div class="output-specification"><p>For each pair of tourists print on a single line a single integer — the time in seconds when the two tourists from the corresponding pair won't see each other. Print the numbers in the order in which the they go in the input.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs of tourists and the number of built walls. The next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> each (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the wall ends and the time it appeared. The last line contains <span class="tex-span"><i>n</i></span> distinct space-separated strictly increasing integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the points of time when pairs of tourists walk.</p><p>All points of time are given in seconds.</p>

## Output

<p>For each pair of tourists print on a single line a single integer — the time in seconds when the two tourists from the corresponding pair won't see each other. Print the numbers in the order in which the they go in the input.</p>





```input1
2 2
1 4 3
3 6 5
0 1

```




```input2
3 3
0 3 4
0 1 2
2 4 0
1 3 4

```




```output1
2
4

```




```output2
2
4
4

```


