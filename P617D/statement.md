## Description

<div><p>There are three points marked on the coordinate plane. The goal is to make a simple polyline, without self-intersections and self-touches, such that it passes through all these points. Also, the polyline must consist of only segments parallel to the coordinate axes. You are to find the minimum number of segments this polyline may consist of.</p></div><div class="input-specification"><p>Each of the three lines of the input contains two integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th point. It is guaranteed that all points are distinct.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the minimum possible number of segments of the polyline.</p></div>

## Input

<p>Each of the three lines of the input contains two integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th point. It is guaranteed that all points are distinct.</p>

## Output

<p>Print a single number&nbsp;— the minimum possible number of segments of the polyline.</p>





```input1
1 -1
1 1
1 2

```




```input2
-1 -1
-1 3
4 3

```




```input3
1 1
2 3
3 2

```




```output1
1

```




```output2
2

```




```output3
3

```



## Note

<p>The variant of the polyline in the first sample: <img class="tex-graphics" src="file://fx9XlNPY.png" style="max-width: 100.0%;max-height: 100.0%;"> The variant of the polyline in the second sample: <img class="tex-graphics" src="file://WsCcYQHZ.png" style="max-width: 100.0%;max-height: 100.0%;"> The variant of the polyline in the third sample: <img class="tex-graphics" src="file://QHraPhnW.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
