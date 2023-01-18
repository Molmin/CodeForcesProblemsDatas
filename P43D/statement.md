## Description

<div><p>The territory of Berland is represented by a rectangular field <span class="tex-span"><i>n</i> × <i>m</i></span> in size. The king of Berland lives in the capital, located on the upper left square <span class="tex-span">(1, 1)</span>. The lower right square has coordinates <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. One day the king decided to travel through the whole country and return back to the capital, having visited every square (except the capital) exactly one time. The king must visit the capital exactly two times, at the very beginning and at the very end of his journey. The king can only move to the side-neighboring squares. However, the royal advise said that the King possibly will not be able to do it. But there is a way out — one can build the system of one way teleporters between some squares so that the king could fulfill his plan. No more than one teleporter can be installed on one square, every teleporter can be used any number of times, however every time it is used, it transports to the same given for any single teleporter square. When the king reaches a square with an installed teleporter he chooses himself whether he is or is not going to use the teleport. What minimum number of teleporters should be installed for the king to complete the journey? You should also compose the journey path route for the king.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100, 2 ≤ </span> <span class="tex-span"><i>n</i></span> <span class="tex-span">·</span> <span class="tex-span"><i>m</i></span>) — the field size. The upper left square has coordinates <span class="tex-span">(1, 1)</span>, and the lower right square has coordinates of <span class="tex-span">(<i>n</i>, <i>m</i>)</span>.</p></div><div class="output-specification"><p>On the first line output integer <span class="tex-span"><i>k</i></span> — the minimum number of teleporters. Then output <span class="tex-span"><i>k</i></span> lines each containing 4 integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the coordinates of the square where the teleporter is installed (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>), and the coordinates of the square where the teleporter leads (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>).</p><p>Then print <span class="tex-span"><i>nm</i> + 1</span> lines containing 2 numbers each — the coordinates of the squares in the order in which they are visited by the king. The travel path must start and end at <span class="tex-span">(1, 1)</span>. The king can move to side-neighboring squares and to the squares where a teleporter leads. Besides, he also should visit the capital exactly two times and he should visit other squares exactly one time.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100, 2 ≤ </span> <span class="tex-span"><i>n</i></span> <span class="tex-span">·</span> <span class="tex-span"><i>m</i></span>) — the field size. The upper left square has coordinates <span class="tex-span">(1, 1)</span>, and the lower right square has coordinates of <span class="tex-span">(<i>n</i>, <i>m</i>)</span>.</p>

## Output

<p>On the first line output integer <span class="tex-span"><i>k</i></span> — the minimum number of teleporters. Then output <span class="tex-span"><i>k</i></span> lines each containing 4 integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the coordinates of the square where the teleporter is installed (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>), and the coordinates of the square where the teleporter leads (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>).</p><p>Then print <span class="tex-span"><i>nm</i> + 1</span> lines containing 2 numbers each — the coordinates of the squares in the order in which they are visited by the king. The travel path must start and end at <span class="tex-span">(1, 1)</span>. The king can move to side-neighboring squares and to the squares where a teleporter leads. Besides, he also should visit the capital exactly two times and he should visit other squares exactly one time.</p>





```input1
2 2

```




```input2
3 3

```




```output1
0
1 1
1 2
2 2
2 1
1 1

```




```output2
1
3 3 1 1
1 1
1 2
1 3
2 3
2 2
2 1
3 1
3 2
3 3
1 1

```


