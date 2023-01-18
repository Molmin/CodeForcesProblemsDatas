## Description

<div><p>There are <span class="tex-span"><i>k</i></span> sensors located in the rectangular room of size <span class="tex-span"><i>n</i> × <i>m</i></span> meters. The <span class="tex-span"><i>i</i></span>-th sensor is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. All sensors are located at distinct points strictly inside the rectangle. </p><p>Opposite corners of the room are located at points <span class="tex-span">(0, 0)</span> and <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Walls of the room are parallel to coordinate axes.</p><p>At the moment <span class="tex-span">0</span>, from the point <span class="tex-span">(0, 0)</span> the laser ray is released in the direction of point <span class="tex-span">(1, 1)</span>. The ray travels with a speed of <img align="middle" class="tex-formula" src="file://AwISkiX9.png" style="max-width: 100.0%;max-height: 100.0%;"> meters per second. Thus, the ray will reach the point <span class="tex-span">(1, 1)</span> in exactly one second after the start.</p><p>When the ray meets the wall it's reflected by the rule that the angle of incidence is equal to the angle of reflection. If the ray reaches any of the four corners, it immediately stops.</p><p>For each sensor you have to determine the first moment of time when the ray will pass through the point where this sensor is located. If the ray will never pass through this point, print <span class="tex-span"> - 1</span> for such sensors.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100 000</span>)&nbsp;— lengths of the room's walls and the number of sensors.</p><p>Each of the following <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i> - 1</span>)&nbsp;— coordinates of the sensors. It's guaranteed that no two sensors are located at the same point.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of seconds when the ray first passes through the point where the <span class="tex-span"><i>i</i></span>-th sensor is located, or <span class="tex-span"> - 1</span> if this will never happen. </p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100 000</span>)&nbsp;— lengths of the room's walls and the number of sensors.</p><p>Each of the following <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i> - 1</span>)&nbsp;— coordinates of the sensors. It's guaranteed that no two sensors are located at the same point.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of seconds when the ray first passes through the point where the <span class="tex-span"><i>i</i></span>-th sensor is located, or <span class="tex-span"> - 1</span> if this will never happen. </p>





```input1
3 3 4
1 1
1 2
2 1
2 2

```




```input2
3 4 6
1 1
2 1
1 2
2 2
1 3
2 3

```




```input3
7 4 5
1 3
2 2
5 1
5 3
4 3

```




```output1
1
-1
-1
2

```




```output2
1
-1
-1
2
5
-1

```




```output3
13
2
9
5
-1

```



## Note

<p>In the first sample, the ray will consequently pass through the points <span class="tex-span">(0, 0)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(3, 3)</span>. Thus, it will stop at the point <span class="tex-span">(3, 3)</span> after <span class="tex-span">3</span> seconds.</p><center> <img class="tex-graphics" height="491px" src="file://dmFUAQIA.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>In the second sample, the ray will consequently pass through the following points: <span class="tex-span">(0, 0)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(3, 3)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(0, 2)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(2, 0)</span>, <span class="tex-span">(3, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(0, 4)</span>. The ray will stop at the point <span class="tex-span">(0, 4)</span> after <span class="tex-span">12</span> seconds. It will reflect at the points <span class="tex-span">(3, 3)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(0, 2)</span>, <span class="tex-span">(2, 0)</span> and <span class="tex-span">(3, 1)</span>.</p><center> <img class="tex-graphics" height="627px" src="file://kict2fhs.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center>
