## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>In good old times dwarves tried to develop extrasensory abilities:</p><ul> <li> Exactly <span class="tex-span"><i>n</i></span> dwarves entered completely dark cave. </li><li> Each dwarf received a hat&nbsp;— white or black. While in cave, none of the dwarves was able to see either his own hat or hats of other Dwarves. </li><li> Dwarves went out of the cave to the meadow and sat at an arbitrary place one after the other. When a dwarf leaves the cave, he sees the colors of all hats of all dwarves that are seating on the meadow (i.e. left the cave before him). However, he is not able to see the color of his own hat and none of the dwarves can give him this information. </li><li> The task for dwarves was to got diverged into two parts&nbsp;— one with dwarves with white hats and one with black hats. </li></ul><p>After many centuries, dwarves finally managed to select the right place on the meadow without error. Will you be able to repeat their success?</p><p>You are asked to successively name <span class="tex-span"><i>n</i></span> different integer points on the plane. After naming each new point you will be given its color&nbsp;— black or white. Your task is to ensure that the named points can be split by a line in such a way that all points of one color lie on the same side from the line and points of different colors lie on different sides. Moreover, no points can belong to the line. Also, you need to report any such line at the end of the process.</p><p>In this problem, the interactor is <span class="tex-font-style-it">adaptive</span>&nbsp;— the colors of the points in the tests are not fixed beforehand and the jury program can select them arbitrarily, in particular, depending on your program output.</p></div><div><h2>Interaction</h2><p>The first line of the standard input stream contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>)&nbsp;— the number of points your program should name.</p><p>Then <span class="tex-span"><i>n</i></span> times your program must print two integer coordinates <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>). All points you print must be distinct.</p><p>In response to each coordinate pair your program will receive the string "<span class="tex-font-style-tt">black</span>", if the point is black, or "<span class="tex-font-style-tt">white</span>", if the point is white.</p><p>When all <span class="tex-span"><i>n</i></span> points are processed, you need to print four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, which form a line, which separates <span class="tex-span"><i>n</i></span> points into black and white. Points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> should not coincide.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack solution use the following format. The first line must contain word "<span class="tex-font-style-tt">hack</span>", the second line should contain the number <span class="tex-span"><i>n</i></span> and the last line should contain the sequence of <span class="tex-span">0</span> and <span class="tex-span">1</span>&nbsp;— colors of points, which will be reported to the solution. Unlike the jury tests, colors of points in hacks are always fixed in advance. Of course, the hacked solution wouldn't be able to get the information about the colors in advance.</p><p>For example, the hack corresponding to sample test will look like this: </p><pre class="verbatim"><br>hack<br>5<br>0 0 1 1 0<br></pre></div>





```input1
5
<span class="tex-span"></span>
black
<span class="tex-span"></span>
black
<span class="tex-span"></span>
white
<span class="tex-span"></span>
white
<span class="tex-span"></span>
black

```




```output1
<span class="tex-span"></span>
0 0
<span class="tex-span"></span>
3 1
<span class="tex-span"></span>
2 3
<span class="tex-span"></span>
4 4
<span class="tex-span"></span>
0 2
<span class="tex-span"></span>
1 3 4 1

```



## Note

<p>In the sample input and output values are aligned only for simplicity of interpreting them chronologically. In real interaction no "extra" line breaks should appear.</p><p>The following picture illustrates the first test.</p><center> <img class="tex-graphics" src="file://WbbHrJyL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
