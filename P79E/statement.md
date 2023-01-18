## Description

<div><p>Fox Ciel safely returned to her castle, but there was something wrong with the security system of the castle: sensors attached in the castle were covering her.</p><p>Ciel is at point <span class="tex-span">(1, 1)</span> of the castle now, and wants to move to point <span class="tex-span">(<i>n</i>, <i>n</i>)</span>, which is the position of her room. By one step, Ciel can move from point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to either <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span> (rightward) or <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span> (upward).</p><p>In her castle, <span class="tex-span"><i>c</i><sup class="upper-index">2</sup></span> sensors are set at points <span class="tex-span">(<i>a</i> + <i>i</i>, <i>b</i> + <i>j</i>)</span> (for every integer <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that: <span class="tex-span">0 ≤ <i>i</i> &lt; <i>c</i>, 0 ≤ <i>j</i> &lt; <i>c</i></span>).</p><p>Each sensor has a count value and decreases its count value every time Ciel moves. Initially, the count value of each sensor is <span class="tex-span"><i>t</i></span>. Every time Ciel moves to point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, the count value of a sensor at point <span class="tex-span">(<i>u</i>, <i>v</i>)</span> decreases by (<span class="tex-span">|<i>u</i> - <i>x</i>| + |<i>v</i> - <i>y</i>|</span>). When the count value of some sensor becomes <span class="tex-font-style-bf">strictly less than</span> <span class="tex-span">0</span>, the sensor will catch Ciel as a suspicious individual!</p><p>Determine whether Ciel can move from <span class="tex-span">(1, 1)</span> to <span class="tex-span">(<i>n</i>, <i>n</i>)</span> without being caught by a sensor, and if it is possible, output her steps. Assume that Ciel can move to every point even if there is a censor on the point.</p></div><div class="input-specification"><p>In the first line there are five integers <span class="tex-span"><i>n</i>, <i>t</i>, <i>a</i>, <i>b</i>, <i>c</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, </span> <span class="tex-span">0 ≤ <i>t</i> ≤ 10<sup class="upper-index">14</sup>, </span> <span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> - <i>c</i> + 1, </span> <span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i> - <i>c</i> + 1, </span> <span class="tex-span">1 ≤ <i>c</i> ≤ <i>n</i></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div><div class="output-specification"><p>If Ciel's objective is possible, output in first line <span class="tex-span">2<i>n</i> - 2</span> characters that represent her feasible steps, where <span class="tex-span"><i>i</i></span>-th character is <span class="tex-font-style-tt">R</span> if <span class="tex-span"><i>i</i></span>-th step is moving rightward, or <span class="tex-font-style-tt">U</span> if moving upward. If there are several solution, output <span class="tex-font-style-bf">lexicographically first</span> one. Character <span class="tex-font-style-tt">R</span> is lexicographically earlier than the character <span class="tex-font-style-tt">U</span>.</p><p>If her objective is impossible, output <span class="tex-font-style-tt">Impossible</span>.</p></div>

## Input

<p>In the first line there are five integers <span class="tex-span"><i>n</i>, <i>t</i>, <i>a</i>, <i>b</i>, <i>c</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, </span> <span class="tex-span">0 ≤ <i>t</i> ≤ 10<sup class="upper-index">14</sup>, </span> <span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> - <i>c</i> + 1, </span> <span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i> - <i>c</i> + 1, </span> <span class="tex-span">1 ≤ <i>c</i> ≤ <i>n</i></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>

## Output

<p>If Ciel's objective is possible, output in first line <span class="tex-span">2<i>n</i> - 2</span> characters that represent her feasible steps, where <span class="tex-span"><i>i</i></span>-th character is <span class="tex-font-style-tt">R</span> if <span class="tex-span"><i>i</i></span>-th step is moving rightward, or <span class="tex-font-style-tt">U</span> if moving upward. If there are several solution, output <span class="tex-font-style-bf">lexicographically first</span> one. Character <span class="tex-font-style-tt">R</span> is lexicographically earlier than the character <span class="tex-font-style-tt">U</span>.</p><p>If her objective is impossible, output <span class="tex-font-style-tt">Impossible</span>.</p>





```input1
5 25 2 4 1

```




```input2
3 6 1 2 2

```




```input3
3 5 1 2 2

```




```input4
20 492 11 4 8

```




```output1
RRUURURU

```




```output2
URUR

```




```output3
Impossible

```




```output4
RRRRRRRRRRRRRRRRUUUUURUUUUURRUUUUUUUUU

```



## Note

<p>The answers for the first sample and the second sample are shown on the picture: </p><center> <img class="tex-graphics" src="file://lMYpdKAH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Here, a red point represents a point that contains a sensor.
