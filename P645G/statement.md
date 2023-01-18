## Description

<div><p>After a drawn-out mooclear arms race, Farmer John and the Mischievous Mess Makers have finally agreed to establish peace. They plan to divide the territory of Bovinia with a line passing through at least two of the <span class="tex-span"><i>n</i></span> outposts scattered throughout the land. These outposts, remnants of the conflict, are located at the points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>), (<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>), ..., (<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>)</span>.</p><p>In order to find the optimal dividing line, Farmer John and Elsie have plotted a map of Bovinia on the coordinate plane. Farmer John's farm and the Mischievous Mess Makers' base are located at the points <span class="tex-span"><i>P</i> = (<i>a</i>, 0)</span> and <span class="tex-span"><i>Q</i> = ( - <i>a</i>, 0)</span>, respectively. Because they seek a lasting peace, Farmer John and Elsie would like to minimize the maximum difference between the distances from any point on the line to <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span>.</p><p>Formally, define the <span class="tex-font-style-bf">difference</span> of a line <img align="middle" class="tex-formula" src="file://89YX0Qh3.png" style="max-width: 100.0%;max-height: 100.0%;"> relative to two points <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> as the smallest real number <span class="tex-span"><i>d</i></span> so that for all points <span class="tex-span"><i>X</i></span> on line <img align="middle" class="tex-formula" src="file://GazqYIh7.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">|<i>PX</i> - <i>QX</i>| ≤ <i>d</i></span>. (It is guaranteed that <span class="tex-span"><i>d</i></span> exists and is unique.) They wish to find the line <img align="middle" class="tex-formula" src="file://esO5rQqY.png" style="max-width: 100.0%;max-height: 100.0%;"> passing through two distinct outposts <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub>)</span> such that the difference of <img align="middle" class="tex-formula" src="file://6APzBTpa.png" style="max-width: 100.0%;max-height: 100.0%;"> relative to <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> is minimized.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>a</i> ≤ 10 000</span>)&nbsp;— the number of outposts and the coordinates of the farm and the base, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines describe the locations of the outposts as pairs of integers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10 000</span>). These points are distinct from each other as well as from <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span>.</p></div><div class="output-specification"><p>Print a single real number—the difference of the optimal dividing line. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://MwGMHHQM.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>a</i> ≤ 10 000</span>)&nbsp;— the number of outposts and the coordinates of the farm and the base, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines describe the locations of the outposts as pairs of integers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10 000</span>). These points are distinct from each other as well as from <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span>.</p>

## Output

<p>Print a single real number—the difference of the optimal dividing line. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://MwGMHHQM.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 5
1 0
2 1

```




```input2
3 6
0 1
2 5
0 -3

```




```output1
7.2111025509

```




```output2
0.0000000000

```



## Note

<p>In the first sample case, the only possible line <img align="middle" class="tex-formula" src="file://4TfOUXJf.png" style="max-width: 100.0%;max-height: 100.0%;"> is <span class="tex-span"><i>y</i> = <i>x</i> - 1</span>. It can be shown that the point <span class="tex-span"><i>X</i></span> which maximizes <span class="tex-span">|<i>PX</i> - <i>QX</i>|</span> is <span class="tex-span">(13, 12)</span>, with <img align="middle" class="tex-formula" src="file://HkLmCTsO.png" style="max-width: 100.0%;max-height: 100.0%;">, which is <img align="middle" class="tex-formula" src="file://vFsE2do2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample case, if we pick the points <span class="tex-span">(0, 1)</span> and <span class="tex-span">(0,  - 3)</span>, we get <img align="middle" class="tex-formula" src="file://g0veyBjS.png" style="max-width: 100.0%;max-height: 100.0%;"> as <span class="tex-span"><i>x</i> = 0</span>. Because <span class="tex-span"><i>PX</i> = <i>QX</i></span> on this line, the minimum possible difference is <span class="tex-span">0</span>.</p>
