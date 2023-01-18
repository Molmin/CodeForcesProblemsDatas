## Description

<div><p>In some country live wizards. They love to ride trolleybuses.</p><p>A city in this country has a trolleybus depot with <span class="tex-span"><i>n</i></span> trolleybuses. Every day the trolleybuses leave the depot, one by one and go to the final station. The final station is at a distance of <span class="tex-span"><i>d</i></span> meters from the depot. We know for the <span class="tex-span"><i>i</i></span>-th trolleybus that it leaves at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> seconds, can go at a speed of no greater than <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> meters per second, and accelerate with an acceleration no greater than <span class="tex-span"><i>a</i></span> meters per second squared. A trolleybus can decelerate as quickly as you want (magic!). It can change its acceleration as fast as you want, as well. Note that the maximum acceleration is the same for all trolleys.</p><p>Despite the magic the trolleys are still powered by an electric circuit and cannot overtake each other (the wires are to blame, of course). If a trolleybus catches up with another one, they go together one right after the other until they arrive at the final station. Also, the drivers are driving so as to arrive at the final station as quickly as possible.</p><p>You, as head of the trolleybuses' fans' club, are to determine for each trolley the minimum time by which it can reach the final station. At the time of arrival at the destination station the trolleybus does not necessarily have zero speed. When a trolley is leaving the depot, its speed is considered equal to zero. From the point of view of physics, the trolleybuses can be considered as material points, and also we should ignore the impact on the speed of a trolley bus by everything, except for the acceleration and deceleration provided by the engine.</p></div><div class="input-specification"><p>The first input line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>d</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of trolleybuses, their maximum acceleration and the distance from the depot to the final station, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub>... &lt; <i>t</i><sub class="lower-index"><i>n</i> - 1</sub> &lt; <i>t</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the time when the <span class="tex-span"><i>i</i></span>-th trolleybus leaves the depot and its maximum speed, correspondingly. The numbers in the lines are separated by spaces.</p></div><div class="output-specification"><p>For each trolleybus print a single line the time it arrives to the final station. Print the times for the trolleybuses in the order in which the trolleybuses are given in the input. The answer will be accepted if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first input line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>d</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of trolleybuses, their maximum acceleration and the distance from the depot to the final station, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub>... &lt; <i>t</i><sub class="lower-index"><i>n</i> - 1</sub> &lt; <i>t</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the time when the <span class="tex-span"><i>i</i></span>-th trolleybus leaves the depot and its maximum speed, correspondingly. The numbers in the lines are separated by spaces.</p>

## Output

<p>For each trolleybus print a single line the time it arrives to the final station. Print the times for the trolleybuses in the order in which the trolleybuses are given in the input. The answer will be accepted if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3 10 10000
0 10
5 11
1000 1

```




```input2
1 2 26
28 29

```




```output1
1000.5000000000
1000.5000000000
11000.0500000000

```




```output2
33.0990195136

```



## Note

<p>In the first sample the second trolleybus will catch up with the first one, that will happen at distance 510.5 meters from the depot. The trolleybuses will go the remaining 9489.5 meters together at speed 10 meters per second. As a result, both trolleybuses will arrive to the final station by the moment of time 1000.5 seconds. The third trolleybus will not catch up with them. It will arrive to the final station by the moment of time 11000.05 seconds.</p>
