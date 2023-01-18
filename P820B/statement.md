## Description

<div><p>On one quiet day all of sudden Mister B decided to draw angle <span class="tex-span"><i>a</i></span> on his field. Aliens have already visited his field and left many different geometric figures on it. One of the figures is <span class="tex-font-style-bf">regular convex <span class="tex-span"><i>n</i></span>-gon</span> (regular convex polygon with <span class="tex-span"><i>n</i></span> sides).</p><p>That's why Mister B decided to use this polygon. Now Mister B must find three distinct vertices <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">3</sub></span> such that the angle <img align="middle" class="tex-formula" src="file://W0DPxUuW.png" style="max-width: 100.0%;max-height: 100.0%;"> (where <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> is the vertex of the angle, and <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">3</sub></span> lie on its sides) is as close as possible to <span class="tex-span"><i>a</i></span>. In other words, the value <img align="middle" class="tex-formula" src="file://rTSp6L2a.png" style="max-width: 100.0%;max-height: 100.0%;"> should be minimum possible.</p><p>If there are many optimal solutions, Mister B should be satisfied with any of them.</p></div><div class="input-specification"><p>First and only line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i> ≤ 180</span>)&nbsp;— the number of vertices in the polygon and the needed angle, in degrees.</p></div><div class="output-specification"><p>Print three space-separated integers: the vertices <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">3</sub></span>, which form <img align="middle" class="tex-formula" src="file://clm1jVaI.png" style="max-width: 100.0%;max-height: 100.0%;">. If there are multiple optimal solutions, print any of them. The vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in clockwise order.</p></div>

## Input

<p>First and only line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i> ≤ 180</span>)&nbsp;— the number of vertices in the polygon and the needed angle, in degrees.</p>

## Output

<p>Print three space-separated integers: the vertices <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">3</sub></span>, which form <img align="middle" class="tex-formula" src="file://clm1jVaI.png" style="max-width: 100.0%;max-height: 100.0%;">. If there are multiple optimal solutions, print any of them. The vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in clockwise order.</p>





```input1
3 15

```




```input2
4 67

```




```input3
4 68

```




```output1
1 2 3

```




```output2
2 1 3

```




```output3
4 1 2

```



## Note

<p>In first sample test vertices of regular triangle can create only angle of <span class="tex-span">60</span> degrees, that's why every possible angle is correct.</p><p>Vertices of square can create <span class="tex-span">45</span> or <span class="tex-span">90</span> degrees angles only. That's why in second sample test the angle of <span class="tex-span">45</span> degrees was chosen, since <span class="tex-span">|45 - 67| &lt; |90 - 67|</span>. Other correct answers are: "3 1 2", "3 2 4", "4 2 3", "4 3 1", "1 3 4", "1 4 2", "2 4 1", "4 1 3", "3 1 4", "3 4 2", "2 4 3", "2 3 1", "1 3 2", "1 2 4", "4 2 1".</p><p>In third sample test, on the contrary, the angle of <span class="tex-span">90</span> degrees was chosen, since <span class="tex-span">|90 - 68| &lt; |45 - 68|</span>. Other correct answers are: "2 1 4", "3 2 1", "1 2 3", "4 3 2", "2 3 4", "1 4 3", "3 4 1".</p>
