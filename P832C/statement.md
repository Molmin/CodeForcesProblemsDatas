## Description

<div><p><span class="tex-span"><i>n</i></span> people are standing on a coordinate axis in points with positive integer coordinates strictly less than <span class="tex-span">10<sup class="upper-index">6</sup></span>. For each person we know in which direction (left or right) he is facing, and his maximum speed.</p><p>You can put a bomb in some point with non-negative integer coordinate, and blow it up. At this moment all people will start running with their maximum speed in the direction they are facing. Also, two strange rays will start propagating from the bomb with speed <span class="tex-span"><i>s</i></span>: one to the right, and one to the left. Of course, the speed <span class="tex-span"><i>s</i></span> is strictly greater than people's maximum speed.</p><p>The rays are strange because if at any moment the position and the direction of movement of some ray and some person coincide, then the speed of the person immediately increases by the speed of the ray.</p><p>You need to place the bomb is such a point that the minimum time moment in which there is a person that has run through point <span class="tex-span">0</span>, and there is a person that has run through point <span class="tex-span">10<sup class="upper-index">6</sup></span>, is as small as possible. In other words, find the minimum time moment <span class="tex-span"><i>t</i></span> such that there is a point you can place the bomb to so that at time moment <span class="tex-span"><i>t</i></span> some person has run through <span class="tex-span">0</span>, and some person has run through point <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of people and the rays' speed.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the description of people. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>s</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>)&nbsp;— the coordinate of the <span class="tex-span"><i>i</i></span>-th person on the line, his maximum speed and the direction he will run to (<span class="tex-span">1</span> is to the left, i.e. in the direction of coordinate decrease, <span class="tex-span">2</span> is to the right, i.e. in the direction of coordinate increase), respectively.</p><p>It is guaranteed that the points <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">6</sup></span> will be reached independently of the bomb's position.</p></div><div class="output-specification"><p>Print the minimum time needed for both points <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">6</sup></span> to be reached.</p><p>Your answer is considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Namely, if your answer is <span class="tex-span"><i>a</i></span>, and the jury's answer is <span class="tex-span"><i>b</i></span>, then your answer is accepted, if <img align="middle" class="tex-formula" src="file://bn1uMcoS.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of people and the rays' speed.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the description of people. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>s</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>)&nbsp;— the coordinate of the <span class="tex-span"><i>i</i></span>-th person on the line, his maximum speed and the direction he will run to (<span class="tex-span">1</span> is to the left, i.e. in the direction of coordinate decrease, <span class="tex-span">2</span> is to the right, i.e. in the direction of coordinate increase), respectively.</p><p>It is guaranteed that the points <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">6</sup></span> will be reached independently of the bomb's position.</p>

## Output

<p>Print the minimum time needed for both points <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">6</sup></span> to be reached.</p><p>Your answer is considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Namely, if your answer is <span class="tex-span"><i>a</i></span>, and the jury's answer is <span class="tex-span"><i>b</i></span>, then your answer is accepted, if <img align="middle" class="tex-formula" src="file://bn1uMcoS.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 999
400000 1 2
500000 1 1

```




```input2
2 1000
400000 500 1
600000 500 2

```




```output1
500000.000000000000000000000000000000

```




```output2
400.000000000000000000000000000000

```



## Note

<p>In the first example, it is optimal to place the bomb at a point with a coordinate of <span class="tex-span">400000</span>. Then at time <span class="tex-span">0</span>, the speed of the first person becomes <span class="tex-span">1000</span> and he reaches the point <span class="tex-span">10<sup class="upper-index">6</sup></span> at the time <span class="tex-span">600</span>. The bomb will not affect on the second person, and he will reach the <span class="tex-span">0</span> point at the time <span class="tex-span">500000</span>.</p><p>In the second example, it is optimal to place the bomb at the point <span class="tex-span">500000</span>. The rays will catch up with both people at the time <span class="tex-span">200</span>. At this time moment, the first is at the point with a coordinate of <span class="tex-span">300000</span>, and the second is at the point with a coordinate of <span class="tex-span">700000</span>. Their speed will become <span class="tex-span">1500</span> and at the time <span class="tex-span">400</span> they will simultaneously run through points <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>
