## Description

<div><p>When the river brought Gerda to the house of the Old Lady who Knew Magic, this lady decided to make Gerda her daughter. She wants Gerda to forget about Kay, so she puts all the roses from the garden underground.</p><p>Mole, who lives in this garden, now can watch the roses without going up to the surface. Typical mole is blind, but this mole was granted as special vision by the Old Lady. He can watch any underground objects on any distance, even through the obstacles and other objects. However, the quality of the picture depends on the Manhattan distance to object being observed.</p><p>Mole wants to find an <span class="tex-font-style-it">optimal</span> point to watch roses, that is such point with <span class="tex-font-style-bf">integer coordinates</span> that the maximum Manhattan distance to the rose is minimum possible.</p><p>As usual, he asks you to help.</p><p><span class="tex-font-style-it">Manhattan distance</span> between points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, &nbsp;<i>y</i><sub class="lower-index">1</sub>, &nbsp;<i>z</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, &nbsp;<i>y</i><sub class="lower-index">2</sub>, &nbsp;<i>z</i><sub class="lower-index">2</sub>)</span> is defined as <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub> - <i>x</i><sub class="lower-index">2</sub>| + |<i>y</i><sub class="lower-index">1</sub> - <i>y</i><sub class="lower-index">2</sub>| + |<i>z</i><sub class="lower-index">1</sub> - <i>z</i><sub class="lower-index">2</sub>|</span>.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100 000</span>)&nbsp;— the number of test cases. Then follow exactly <span class="tex-span"><i>t</i></span> blocks, each containing the description of exactly one test.</p><p>The first line of each block contains an integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the number of roses in the test. Then follow <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> lines, containing three integers each&nbsp;— the coordinates of the corresponding rose. Note that two or more roses may share the same position.</p><p>It's guaranteed that the sum of all <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">100 000</span> and all coordinates are not greater than <span class="tex-span">10<sup class="upper-index">18</sup></span> by their absolute value.</p></div><div class="output-specification"><p>For each of <span class="tex-span"><i>t</i></span> test cases print three integers&nbsp;— the coordinates of the optimal point to watch roses. If there are many optimal answers, print any of them.</p><p>The coordinates of the optimal point may coincide with the coordinates of any rose.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100 000</span>)&nbsp;— the number of test cases. Then follow exactly <span class="tex-span"><i>t</i></span> blocks, each containing the description of exactly one test.</p><p>The first line of each block contains an integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the number of roses in the test. Then follow <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> lines, containing three integers each&nbsp;— the coordinates of the corresponding rose. Note that two or more roses may share the same position.</p><p>It's guaranteed that the sum of all <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">100 000</span> and all coordinates are not greater than <span class="tex-span">10<sup class="upper-index">18</sup></span> by their absolute value.</p>

## Output

<p>For each of <span class="tex-span"><i>t</i></span> test cases print three integers&nbsp;— the coordinates of the optimal point to watch roses. If there are many optimal answers, print any of them.</p><p>The coordinates of the optimal point may coincide with the coordinates of any rose.</p>





```input1
1
5
0 0 4
0 0 -4
0 4 0
4 0 0
1 1 1

```




```input2
2
1
3 5 9
2
3 5 9
3 5 9

```




```output1
0 0 0

```




```output2
3 5 9
3 5 9

```



## Note

<p>In the first sample, the maximum Manhattan distance from the point to the rose is equal to <span class="tex-span">4</span>.</p><p>In the second sample, the maximum possible distance is <span class="tex-span">0</span>. Note that the positions of the roses may coincide with each other and with the position of the optimal point.</p>
