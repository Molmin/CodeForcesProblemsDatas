## Description

<div><p>Emuskald was hired to design an artificial waterfall according to the latest trends in landscape architecture. A modern artificial waterfall consists of multiple horizontal panels affixed to a wide flat wall. The water flows down the top of the wall from panel to panel until it reaches the bottom of the wall.</p><p>The wall has height <span class="tex-span"><i>t</i></span> and has <span class="tex-span"><i>n</i></span> panels on the wall. Each panel is a horizontal segment at height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> which begins at <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and ends at <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th panel connects the points <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub>)</span> and <span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub>)</span> of the plane. The top of the wall can be considered a panel connecting the points <span class="tex-span">( - 10<sup class="upper-index">9</sup>, <i>t</i>)</span> and <span class="tex-span">(10<sup class="upper-index">9</sup>, <i>t</i>)</span>. Similarly, the bottom of the wall can be considered a panel connecting the points <span class="tex-span">( - 10<sup class="upper-index">9</sup>, 0)</span> and <span class="tex-span">(10<sup class="upper-index">9</sup>, 0)</span>. No two panels share a common point.</p><p>Emuskald knows that for the waterfall to be aesthetically pleasing, it can flow from panel <span class="tex-span"><i>i</i></span> to panel <span class="tex-span"><i>j</i></span> (<img align="middle" class="tex-formula" src="file://XhZTuV9A.png" style="max-width: 100.0%;max-height: 100.0%;">) only if the following conditions hold: </p><ol> <li> <span class="tex-span"><i>max</i>(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>j</i></sub>) &lt; <i>min</i>(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>)</span> (horizontal projections of the panels overlap); </li><li> <span class="tex-span"><i>h</i><sub class="lower-index"><i>j</i></sub> &lt; <i>h</i><sub class="lower-index"><i>i</i></sub></span> (panel <span class="tex-span"><i>j</i></span> is below panel <span class="tex-span"><i>i</i></span>); </li><li> there is no such panel <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>h</i><sub class="lower-index"><i>j</i></sub> &lt; <i>h</i><sub class="lower-index"><i>k</i></sub> &lt; <i>h</i><sub class="lower-index"><i>i</i></sub>)</span> that the first two conditions hold for the pairs <span class="tex-span">(<i>i</i>, <i>k</i>)</span> and <span class="tex-span">(<i>k</i>, <i>j</i>)</span>. </li></ol><p>Then the <span class="tex-font-style-bf">flow</span> for <img align="middle" class="tex-formula" src="file://1yzpTtxw.png" style="max-width: 100.0%;max-height: 100.0%;"> is equal to <span class="tex-span"><i>min</i>(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>) - <i>max</i>(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>j</i></sub>)</span>, the length of their horizontal projection overlap.</p><p>Emuskald has decided that in his waterfall the water will flow in a single path from top to bottom. If water flows to a panel (except the bottom of the wall), the water will fall further to <span class="tex-font-style-bf">exactly one</span> lower panel. The total amount of water flow in the waterfall is then defined as the minimum horizontal projection overlap between two consecutive panels in the path of the waterfall. Formally: </p><ol> <li> the waterfall consists of a single path of panels <img align="middle" class="tex-formula" src="file://qWGRpLPP.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> the flow of the waterfall is the minimum flow in the path <img align="middle" class="tex-formula" src="file://opKg9XbA.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol><p> To make a truly great waterfall Emuskald must maximize this water flow, but there are too many panels and he is having a hard time planning his creation. Below is an example of a waterfall Emuskald wants:</p><center> <img class="tex-graphics" src="file://UVH7Z0EW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help Emuskald maintain his reputation and find the value of the maximum possible water flow.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>), the number of the panels excluding the top and the bottom panels, and the height of the wall. Each of the <span class="tex-span"><i>n</i></span> following lines contain three space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>h</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the height, left and right ends of the <span class="tex-span"><i>i</i></span>-th panel segment.</p><p>It is guaranteed that no two segments share a common point.</p></div><div class="output-specification"><p>Output a single integer — the maximum possible amount of water flow in the desired waterfall.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>), the number of the panels excluding the top and the bottom panels, and the height of the wall. Each of the <span class="tex-span"><i>n</i></span> following lines contain three space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>h</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the height, left and right ends of the <span class="tex-span"><i>i</i></span>-th panel segment.</p><p>It is guaranteed that no two segments share a common point.</p>

## Output

<p>Output a single integer — the maximum possible amount of water flow in the desired waterfall.</p>





```input1
5 6
4 1 6
3 2 7
5 9 11
3 10 15
1 13 16

```




```input2
6 5
4 2 8
3 1 2
2 2 3
2 6 12
1 0 7
1 8 11

```




```output1
4

```




```output2
2

```



## Note

<p>The first test case corresponds to the picture.</p>
