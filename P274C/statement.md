## Description

<div><p>Luyi has <span class="tex-span"><i>n</i></span> circles on the plane. The <span class="tex-span"><i>i</i></span>-th circle is centered at <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. At the time zero circles start to grow simultaneously. In other words, the radius of each circle at time <span class="tex-span"><i>t</i> (<i>t</i> &gt; 0)</span> is equal to <span class="tex-span"><i>t</i></span>. The circles are drawn as black discs on an infinite white plane. So at each moment the plane consists of several black and white regions. Note that the circles may overlap while growing.</p><center> <img class="tex-graphics" src="file://EW1kEXkb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We define a <span class="tex-font-style-underline">hole</span> as a closed, connected white region. For instance, the figure contains two holes shown by red border. During growing some holes may be created and it is easy to see that each created hole will disappear eventually. Luyi asks you to find moment of time such that the last hole disappears. In other words, you should find the first moment such that no hole can be seen after that.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), indicating the location of <span class="tex-span"><i>i</i></span>-th circle.</p><p>It's guaranteed that no two circles are centered at the same point.</p></div><div class="output-specification"><p>Print the moment where the last hole disappears. If there exists no moment in which we can find holes print <span class="tex-font-style-tt">-1</span>.</p><p>The answer will be considered correct if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), indicating the location of <span class="tex-span"><i>i</i></span>-th circle.</p><p>It's guaranteed that no two circles are centered at the same point.</p>

## Output

<p>Print the moment where the last hole disappears. If there exists no moment in which we can find holes print <span class="tex-font-style-tt">-1</span>.</p><p>The answer will be considered correct if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3
0 0
1 1
2 2

```




```input2
4
0 0
0 2
2 2
2 0

```




```input3
4
0 1
0 -1
-2 0
4 0

```




```output1
-1

```




```output2
1.414214

```




```output3
2.125000

```


