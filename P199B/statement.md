## Description

<div><p>A renowned abstract artist Sasha, drawing inspiration from nowhere, decided to paint a picture entitled "Special Olympics". He justly thought that, if the regular Olympic games have five rings, then the Special ones will do with exactly two rings just fine.</p><p>Let us remind you that a ring is a region located between two concentric circles with radii <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>R</i></span> <span class="tex-span">(<i>r</i> &lt; <i>R</i>)</span>. These radii are called internal and external, respectively. Concentric circles are circles with centers located at the same point.</p><p>Soon a white canvas, which can be considered as an infinite Cartesian plane, had two perfect rings, painted with solid black paint. As Sasha is very impulsive, the rings could have different radii and sizes, they intersect and overlap with each other in any way. We know only one thing for sure: the centers of the pair of rings are not the same.</p><p>When Sasha got tired and fell into a deep sleep, a girl called Ilona came into the room and wanted to cut a circle for the sake of good memories. To make the circle beautiful, she decided to cut along the contour.</p><p>We'll consider a contour to be a continuous closed line through which there is transition from one color to another (see notes for clarification). If the contour takes the form of a circle, then the result will be cutting out a circle, which Iona wants.</p><p>But the girl's inquisitive mathematical mind does not rest: how many ways are there to cut a circle out of the canvas?</p></div><div class="input-specification"><p>The input contains two lines. </p><p>Each line has four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span>, that describe the <span class="tex-span"><i>i</i></span>-th ring; <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are coordinates of the ring's center, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> are the internal and external radii of the ring correspondingly <span class="tex-span">( - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100;&nbsp;1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> &lt; <i>R</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. </p><p>It is guaranteed that the centers of the rings do not coinside.</p></div><div class="output-specification"><p>A single integer — the number of ways to cut out a circle from the canvas.</p></div>

## Input

<p>The input contains two lines. </p><p>Each line has four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span>, that describe the <span class="tex-span"><i>i</i></span>-th ring; <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are coordinates of the ring's center, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> are the internal and external radii of the ring correspondingly <span class="tex-span">( - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100;&nbsp;1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> &lt; <i>R</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. </p><p>It is guaranteed that the centers of the rings do not coinside.</p>

## Output

<p>A single integer — the number of ways to cut out a circle from the canvas.</p>





```input1
60 60 45 55
80 80 8 32

```




```input2
60 60 45 55
80 60 15 25

```




```input3
50 50 35 45
90 50 35 45

```




```output1
1
```




```output2
4
```




```output3
0
```



## Note

<p>Figures for test samples are given below. The possible cuts are marked with red dotted line. </p><center> <img class="tex-graphics" src="file://pPTXqMj8.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://XssdNGoZ.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://ikxz4bO2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
