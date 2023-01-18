## Description

<div><p>Once Danil the student was returning home from tram stop lately by straight road of length <span class="tex-span"><i>L</i></span>. The stop is located at the point <span class="tex-span"><i>x</i> = 0</span>, but the Danil's home&nbsp;— at the point <span class="tex-span"><i>x</i> = <i>L</i></span>. Danil goes from <span class="tex-span"><i>x</i> = 0</span> to <span class="tex-span"><i>x</i> = <i>L</i></span> with a constant speed and does not change direction of movement.</p><p>There are <span class="tex-span"><i>n</i></span> street lights at the road, each of which lights some continuous segment of the road. All of the <span class="tex-span"><i>n</i></span> lightened segments do not share common points.</p><p>Danil loves to sing, thus he wants to sing his favourite song over and over again during his walk. As soon as non-lightened segments of the road scare him, he sings only when he goes through the lightened segments.</p><p>Danil passes distance <span class="tex-span"><i>p</i></span> while performing his favourite song once. Danil can't start another performance if the segment passed while performing is not fully lightened. Moreover, if Danil has taken a pause between two performances, he is not performing while not having passed a segment of length at least <span class="tex-span"><i>t</i></span>. Formally,</p><ol> <li> Danil can start single performance at a point <span class="tex-span"><i>x</i></span> only if every point of segment <span class="tex-span">[<i>x</i>, <i>x</i> + <i>p</i>]</span> is lightened; </li><li> If Danil has finished performing at a point <span class="tex-span"><i>x</i> + <i>p</i></span>, then the next performance can be started only at a point <span class="tex-span"><i>y</i></span> such that <span class="tex-span"><i>y</i> = <i>x</i> + <i>p</i></span> or <span class="tex-span"><i>y</i> ≥ <i>x</i> + <i>p</i> + <i>t</i></span> satisfying the statement under the point <span class="tex-span">1</span>. </li></ol><center> <img class="tex-graphics" src="file://I6b9diE9.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Blue half-circles denote performances. Please note that just after Danil has taken a pause in performing, he has not sang for a path of length of at least <span class="tex-span"><i>t</i></span>.</span> </center><p>Determine how many times Danil can perform his favourite song during his walk from <span class="tex-span"><i>x</i> = 0</span> to <span class="tex-span"><i>x</i> = <i>L</i></span>.</p><p>Please note that Danil does not break a single performance, thus, started singing another time, he finishes singing when having a segment of length of <span class="tex-span"><i>p</i></span> passed from the performance start point.</p></div><div class="input-specification"><p>The first line of the input contains four integers <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the Danil's path, the number of street lights at the road, the distance Danil passes while doing single performance and the minimum distance of pause respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe segments lightened by street lights. <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>)&nbsp;— the endpoints of the segment lightened by <span class="tex-span"><i>i</i></span>-th street light. It is guaranteed that no two segments are intersecting, nesting, or touching each other. The segments are given in the order from left to right.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the maximum number of performances of Danil's favourite song on the path from <span class="tex-span"><i>x</i> = 0</span> to <span class="tex-span"><i>x</i> = <i>L</i></span>.</p></div>

## Input

<p>The first line of the input contains four integers <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the Danil's path, the number of street lights at the road, the distance Danil passes while doing single performance and the minimum distance of pause respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe segments lightened by street lights. <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>)&nbsp;— the endpoints of the segment lightened by <span class="tex-span"><i>i</i></span>-th street light. It is guaranteed that no two segments are intersecting, nesting, or touching each other. The segments are given in the order from left to right.</p>

## Output

<p>Print the only integer&nbsp;— the maximum number of performances of Danil's favourite song on the path from <span class="tex-span"><i>x</i> = 0</span> to <span class="tex-span"><i>x</i> = <i>L</i></span>.</p>





```input1
17 2 2 6
0 9
13 17

```




```input2
12 2 2 2
0 5
6 11

```




```input3
12 2 2 4
0 5
6 11

```




```output1
5

```




```output2
4

```




```output3
3

```



## Note

<p>The first sample case is just about corresponding to the picture from the statement.</p>
