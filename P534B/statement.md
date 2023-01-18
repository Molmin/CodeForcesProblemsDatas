## Description

<div><p>The on-board computer on Polycarp's car measured that the car speed at the beginning of some section of the path equals <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> meters per second, and in the end it is <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> meters per second. We know that this section of the route took exactly <span class="tex-span"><i>t</i></span> seconds to pass.</p><p>Assuming that at each of the seconds the speed is constant, and between seconds the speed can change at most by <span class="tex-span"><i>d</i></span> meters per second in absolute value (i.e., the difference in the speed of any two adjacent seconds does not exceed <span class="tex-span"><i>d</i></span> in absolute value), find the maximum possible length of the path section in meters.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ 100</span>) — the speeds in meters per second at the beginning of the segment and at the end of the segment, respectively.</p><p>The second line contains two integers <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>t</i> ≤ 100</span>) — the time when the car moves along the segment in seconds, <span class="tex-span"><i>d</i></span> <span class="tex-font-style-bf"><span class="tex-span">(0 ≤ <i>d</i> ≤ 10)</span></span> — the maximum value of the speed change between adjacent seconds.</p><p>It is guaranteed that there is a way to complete the segment so that:</p><ul> <li> the speed in the first second equals <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, </li><li> the speed in the last second equals <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, </li><li> the absolute value of difference of speeds between any two adjacent seconds doesn't exceed <span class="tex-span"><i>d</i></span>. </li></ul></div><div class="output-specification"><p>Print the maximum possible length of the path segment in meters. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ 100</span>) — the speeds in meters per second at the beginning of the segment and at the end of the segment, respectively.</p><p>The second line contains two integers <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>t</i> ≤ 100</span>) — the time when the car moves along the segment in seconds, <span class="tex-span"><i>d</i></span> <span class="tex-font-style-bf"><span class="tex-span">(0 ≤ <i>d</i> ≤ 10)</span></span> — the maximum value of the speed change between adjacent seconds.</p><p>It is guaranteed that there is a way to complete the segment so that:</p><ul> <li> the speed in the first second equals <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, </li><li> the speed in the last second equals <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, </li><li> the absolute value of difference of speeds between any two adjacent seconds doesn't exceed <span class="tex-span"><i>d</i></span>. </li></ul>

## Output

<p>Print the maximum possible length of the path segment in meters. </p>





```input1
5 6
4 2

```




```input2
10 10
10 0

```




```output1
26
```




```output2
100
```



## Note

<p>In the first sample the sequence of speeds of Polycarpus' car can look as follows: 5, 7, 8, 6. Thus, the total path is <span class="tex-span">5 + 7 + 8 + 6 = 26</span> meters.</p><p>In the second sample, as <span class="tex-span"><i>d</i> = 0</span>, the car covers the whole segment at constant speed <span class="tex-span"><i>v</i> = 10</span>. In <span class="tex-span"><i>t</i> = 10</span> seconds it covers the distance of 100 meters.</p>
