## Description

<div><p>A car moves from point A to point B at speed <span class="tex-span"><i>v</i></span> meters per second. The action takes place on the X-axis. At the distance <span class="tex-span"><i>d</i></span> meters from A there are traffic lights. Starting from time 0, for the first <span class="tex-span"><i>g</i></span> seconds the green light is on, then for the following <span class="tex-span"><i>r</i></span> seconds the red light is on, then again the green light is on for the <span class="tex-span"><i>g</i></span> seconds, and so on.</p><p>The car can be instantly accelerated from <span class="tex-span">0</span> to <span class="tex-span"><i>v</i></span> and vice versa, can instantly slow down from the <span class="tex-span"><i>v</i></span> to <span class="tex-span">0</span>. Consider that it passes the traffic lights at the green light instantly. If the car approaches the traffic lights at the moment when the red light has just turned on, it doesn't have time to pass it. But if it approaches the traffic lights at the moment when the green light has just turned on, it can move. The car leaves point A at the time 0.</p><p>What is the minimum time for the car to get from point A to point B without breaking the traffic rules?</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>g</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i>, <i>d</i>, <i>v</i>, <i>g</i>, <i>r</i> ≤ 1000, <i>d</i> &lt; <i>l</i></span>) — the distance between A and B (in meters), the distance from A to the traffic lights, car's speed, the duration of green light and the duration of red light.</p></div><div class="output-specification"><p>Output a single number — the minimum time that the car needs to get from point A to point B. Your output must have relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>g</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i>, <i>d</i>, <i>v</i>, <i>g</i>, <i>r</i> ≤ 1000, <i>d</i> &lt; <i>l</i></span>) — the distance between A and B (in meters), the distance from A to the traffic lights, car's speed, the duration of green light and the duration of red light.</p>

## Output

<p>Output a single number — the minimum time that the car needs to get from point A to point B. Your output must have relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 1 3 4 5

```




```input2
5 4 3 1 1

```




```output1
0.66666667

```




```output2
2.33333333

```


