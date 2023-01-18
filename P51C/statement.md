## Description

<div><p>The New Vasjuki village is stretched along the motorway and that's why every house on it is characterized by its shift relative to some fixed point — the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coordinate. The village consists of <span class="tex-span"><i>n</i></span> houses, the <span class="tex-span"><i>i</i></span>-th house is located in the point with coordinates of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>TELE3, a cellular communication provider planned to locate three base stations so as to provide every house in the village with cellular communication. The base station having power <span class="tex-span"><i>d</i></span> located in the point <span class="tex-span"><i>t</i></span> provides with communication all the houses on the segment <span class="tex-span">[<i>t</i> - <i>d</i>, <i>t</i> + <i>d</i>]</span> (including boundaries).</p><p>To simplify the integration (and simply not to mix anything up) all the three stations are planned to possess the equal power of <span class="tex-span"><i>d</i></span>. Which minimal value of <span class="tex-span"><i>d</i></span> is enough to provide all the houses in the village with cellular communication.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) which represents the number of houses in the village. The second line contains the coordinates of houses — the sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> of integer numbers (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It is possible that two or more houses are located on one point. The coordinates are given in a arbitrary order.</p></div><div class="output-specification"><p>Print the required minimal power <span class="tex-span"><i>d</i></span>. In the second line print three numbers — the possible coordinates of the base stations' location. Print the coordinates with 6 digits after the decimal point. The positions of the stations can be any from <span class="tex-span">0</span> to <span class="tex-span">2·10<sup class="upper-index">9</sup></span> inclusively. It is accepted for the base stations to have matching coordinates. If there are many solutions, print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) which represents the number of houses in the village. The second line contains the coordinates of houses — the sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> of integer numbers (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It is possible that two or more houses are located on one point. The coordinates are given in a arbitrary order.</p>

## Output

<p>Print the required minimal power <span class="tex-span"><i>d</i></span>. In the second line print three numbers — the possible coordinates of the base stations' location. Print the coordinates with 6 digits after the decimal point. The positions of the stations can be any from <span class="tex-span">0</span> to <span class="tex-span">2·10<sup class="upper-index">9</sup></span> inclusively. It is accepted for the base stations to have matching coordinates. If there are many solutions, print any of them.</p>





```input1
4
1 2 3 4

```




```input2
3
10 20 30

```




```input3
5
10003 10004 10001 10002 1

```




```output1
0.500000
1.500000 2.500000 3.500000

```




```output2
0
10.000000 20.000000 30.000000

```




```output3
0.500000
1.000000 10001.500000 10003.500000

```


