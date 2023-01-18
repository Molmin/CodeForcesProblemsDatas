## Description

<div><p>A team of furry rescue rangers was sitting idle in their hollow tree when suddenly they received a signal of distress. In a few moments they were ready, and the dirigible of the rescue chipmunks hit the road.</p><p>We assume that the action takes place on a Cartesian plane. The headquarters of the rescuers is located at point <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, and the distress signal came from the point <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>Due to Gadget's engineering talent, the rescuers' dirigible can instantly change its current velocity and direction of movement at any moment and as many times as needed. The only limitation is: the speed of the aircraft relative to the air can not exceed <img align="middle" class="tex-formula" src="file://WwVokUUl.png" style="max-width: 100.0%;max-height: 100.0%;"> meters per second.</p><p>Of course, Gadget is a true rescuer and wants to reach the destination as soon as possible. The matter is complicated by the fact that the wind is blowing in the air and it affects the movement of the dirigible. According to the weather forecast, the wind will be defined by the vector <span class="tex-span">(<i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>)</span> for the nearest <span class="tex-span"><i>t</i></span> seconds, and then will change to <span class="tex-span">(<i>w</i><sub class="lower-index"><i>x</i></sub>, <i>w</i><sub class="lower-index"><i>y</i></sub>)</span>. These vectors give both the direction and velocity of the wind. Formally, if a dirigible is located at the point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, while its own velocity relative to the air is equal to zero and the wind <span class="tex-span">(<i>u</i><sub class="lower-index"><i>x</i></sub>, <i>u</i><sub class="lower-index"><i>y</i></sub>)</span> is blowing, then after <img align="middle" class="tex-formula" src="file://aagrxjzu.png" style="max-width: 100.0%;max-height: 100.0%;"> seconds the new position of the dirigible will be <img align="middle" class="tex-formula" src="file://rakwWGUg.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Gadget is busy piloting the aircraft, so she asked Chip to calculate how long will it take them to reach the destination if they fly optimally. He coped with the task easily, but Dale is convinced that Chip has given the random value, aiming only not to lose the face in front of Gadget. Dale has asked you to find the right answer.</p><p>It is guaranteed that the speed of the wind at any moment of time is strictly less than the maximum possible speed of the airship relative to the air.</p></div><div class="input-specification"><p>The first line of the input contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index">1</sub>|,  |<i>y</i><sub class="lower-index">1</sub>|,  |<i>x</i><sub class="lower-index">2</sub>|,  |<i>y</i><sub class="lower-index">2</sub>| ≤ 10 000</span>)&nbsp;— the coordinates of the rescuers' headquarters and the point, where signal of the distress came from, respectively. </p><p>The second line contains two integers <img align="middle" class="tex-formula" src="file://lOEcXSAM.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 &lt; <i>v</i>, <i>t</i> ≤ 1000</span>), which are denoting the maximum speed of the chipmunk dirigible relative to the air and the moment of time when the wind changes according to the weather forecast, respectively. </p><p>Next follow one per line two pairs of integer <span class="tex-span">(<i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>)</span> and <span class="tex-span">(<i>w</i><sub class="lower-index"><i>x</i></sub>, <i>w</i><sub class="lower-index"><i>y</i></sub>)</span>, describing the wind for the first <span class="tex-span"><i>t</i></span> seconds and the wind that will blow at all the remaining time, respectively. It is guaranteed that <img align="middle" class="tex-formula" src="file://Tjz48YtL.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://bKGSgtsE.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Print a single real value&nbsp;— the minimum time the rescuers need to get to point <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://IzUORifa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index">1</sub>|,  |<i>y</i><sub class="lower-index">1</sub>|,  |<i>x</i><sub class="lower-index">2</sub>|,  |<i>y</i><sub class="lower-index">2</sub>| ≤ 10 000</span>)&nbsp;— the coordinates of the rescuers' headquarters and the point, where signal of the distress came from, respectively. </p><p>The second line contains two integers <img align="middle" class="tex-formula" src="file://lOEcXSAM.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 &lt; <i>v</i>, <i>t</i> ≤ 1000</span>), which are denoting the maximum speed of the chipmunk dirigible relative to the air and the moment of time when the wind changes according to the weather forecast, respectively. </p><p>Next follow one per line two pairs of integer <span class="tex-span">(<i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>)</span> and <span class="tex-span">(<i>w</i><sub class="lower-index"><i>x</i></sub>, <i>w</i><sub class="lower-index"><i>y</i></sub>)</span>, describing the wind for the first <span class="tex-span"><i>t</i></span> seconds and the wind that will blow at all the remaining time, respectively. It is guaranteed that <img align="middle" class="tex-formula" src="file://Tjz48YtL.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://bKGSgtsE.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Print a single real value&nbsp;— the minimum time the rescuers need to get to point <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://IzUORifa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
0 0 5 5
3 2
-1 -1
-1 0

```




```input2
0 0 0 1000
100 1000
-50 0
50 0

```




```output1
3.729935587093555327

```




```output2
11.547005383792516398

```


