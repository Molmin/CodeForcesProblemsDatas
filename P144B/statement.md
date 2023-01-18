## Description

<div><p>The Super Duper Secret Meeting of the Super Duper Secret Military Squad takes place in a Super Duper Secret Place. The place is an infinite plane with introduced Cartesian coordinate system. The meeting table is represented as a rectangle whose sides are parallel to the coordinate axes and whose vertexes are located at the integer points of the plane. At each integer point which belongs to the table perimeter there is a chair in which a general sits.</p><p>Some points on the plane contain radiators for the generals not to freeze in winter. Each radiator is characterized by the number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the radius of the area this radiator can heat. That is, if the distance between some general and the given radiator is less than or equal to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, than the general feels comfortable and warm. Here distance is defined as Euclidean distance, so the distance between points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> is <img align="middle" class="tex-formula" src="file://avdKcvot.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Each general who is located outside the radiators' heating area can get sick. Thus, you should bring him a warm blanket. Your task is to count the number of warm blankets you should bring to the Super Duper Secret Place.</p><p>The generals who are already comfortable do not need a blanket. Also the generals never overheat, ever if they are located in the heating area of several radiators. The radiators can be located at any integer points on the plane, even inside the rectangle (under the table) or on the perimeter (directly under some general). Even in this case their radius does not change.</p></div><div class="input-specification"><p>The first input line contains coordinates of two opposite table corners <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub> ≠ <i>x</i><sub class="lower-index"><i>b</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub> ≠ <i>y</i><sub class="lower-index"><i>b</i></sub>)</span>. The second line contains integer <span class="tex-span"><i>n</i></span> — the number of radiators (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>). Then <span class="tex-span"><i>n</i></span> lines contain the heaters' coordinates as "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span></span>", the numbers are separated by spaces. All input data numbers are integers. The absolute value of all coordinates does not exceed <span class="tex-span">1000</span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>. Several radiators can be located at the same point.</p></div><div class="output-specification"><p>Print the only number — the number of blankets you should bring.</p></div>

## Input

<p>The first input line contains coordinates of two opposite table corners <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub> ≠ <i>x</i><sub class="lower-index"><i>b</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub> ≠ <i>y</i><sub class="lower-index"><i>b</i></sub>)</span>. The second line contains integer <span class="tex-span"><i>n</i></span> — the number of radiators (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>). Then <span class="tex-span"><i>n</i></span> lines contain the heaters' coordinates as "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span></span>", the numbers are separated by spaces. All input data numbers are integers. The absolute value of all coordinates does not exceed <span class="tex-span">1000</span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>. Several radiators can be located at the same point.</p>

## Output

<p>Print the only number — the number of blankets you should bring.</p>





```input1
2 5 4 2
3
3 1 2
5 3 1
1 3 2

```




```input2
5 2 6 3
2
6 2 2
6 5 3

```




```output1
4

```




```output2
0

```



## Note

<p>In the first sample the generals are sitting at points: <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(2, 5)</span>, <span class="tex-span">(3, 2)</span>, <span class="tex-span">(3, 5)</span>, <span class="tex-span">(4, 2)</span>, <span class="tex-span">(4, 3)</span>, <span class="tex-span">(4, 4)</span>, <span class="tex-span">(4, 5)</span>. Among them, 4 generals are located outside the heating range. They are the generals at points: <span class="tex-span">(2, 5)</span>, <span class="tex-span">(3, 5)</span>, <span class="tex-span">(4, 4)</span>, <span class="tex-span">(4, 5)</span>.</p><p>In the second sample the generals are sitting at points: <span class="tex-span">(5, 2)</span>, <span class="tex-span">(5, 3)</span>, <span class="tex-span">(6, 2)</span>, <span class="tex-span">(6, 3)</span>. All of them are located inside the heating range.</p>
