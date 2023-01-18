## Description

<div><p>In this problem we assume the Earth to be a completely round ball and its surface a perfect sphere. The length of the equator and any meridian is considered to be exactly <span class="tex-span">40 000</span> kilometers. Thus, travelling from North Pole to South Pole or vice versa takes exactly <span class="tex-span">20 000</span> kilometers.</p><p>Limak, a polar bear, lives on the North Pole. Close to the New Year, he helps somebody with delivering packages all around the world. Instead of coordinates of places to visit, Limak got a description how he should move, assuming that he starts from the North Pole. The description consists of <span class="tex-span"><i>n</i></span> parts. In the <span class="tex-span"><i>i</i></span>-th part of his journey, Limak should move <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> kilometers in the direction represented by a string <span class="tex-span"><i>dir</i><sub class="lower-index"><i>i</i></sub></span> that is one of: "<span class="tex-font-style-tt">North</span>", "<span class="tex-font-style-tt">South</span>", "<span class="tex-font-style-tt">West</span>", "<span class="tex-font-style-tt">East</span>".</p><p>Limak isn’t sure whether the description is valid. You must help him to check the following conditions:</p><ul> <li> If at any moment of time (before any of the instructions or while performing one of them) Limak is on the North Pole, he can move only to the South. </li><li> If at any moment of time (before any of the instructions or while performing one of them) Limak is on the South Pole, he can move only to the North. </li><li> The journey must end on the North Pole. </li></ul><p>Check if the above conditions are satisfied and print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" on a single line.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>).</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and a string <span class="tex-span"><i>dir</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <img align="middle" class="tex-formula" src="file://VJrXf4oN.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the length and the direction of the <span class="tex-span"><i>i</i></span>-th part of the journey, according to the description Limak got.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if the description satisfies the three conditions, otherwise print "<span class="tex-font-style-tt">NO</span>", both without the quotes.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>).</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and a string <span class="tex-span"><i>dir</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <img align="middle" class="tex-formula" src="file://VJrXf4oN.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the length and the direction of the <span class="tex-span"><i>i</i></span>-th part of the journey, according to the description Limak got.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if the description satisfies the three conditions, otherwise print "<span class="tex-font-style-tt">NO</span>", both without the quotes.</p>





```input1
5
7500 South
10000 East
3500 North
4444 West
4000 North

```




```input2
2
15000 South
4000 East

```




```input3
5
20000 South
1000 North
1000000 West
9000 North
10000 North

```




```input4
3
20000 South
10 East
20000 North

```




```input5
2
1000 North
1000 South

```




```input6
4
50 South
50 North
15000 South
15000 North

```




```output1
YES

```




```output2
NO

```




```output3
YES

```




```output4
NO

```




```output5
NO

```




```output6
YES

```



## Note

<p>Drawings below show how Limak's journey would look like in first two samples. In the second sample the answer is "<span class="tex-font-style-tt">NO</span>" because he doesn't end on the North Pole.</p><center> <img class="tex-graphics" src="file://B113XRCH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
