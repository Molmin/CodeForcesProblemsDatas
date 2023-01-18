## Description

<div><p>On a number line there are <span class="tex-span"><i>n</i></span> balls. At time moment <span class="tex-span">0</span> for each ball the following data is known: its coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (possibly, negative) and weight <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>. The radius of the balls can be ignored.</p><p>The balls collide elastically, i.e. if two balls weighing <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> and with speeds <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> collide, their new speeds will be: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://Zi7da5me.png" style="max-width: 100.0%;max-height: 100.0%;"></center>.<p>Your task is to find out, where each ball will be <span class="tex-span"><i>t</i></span> seconds after.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10, 0 ≤ <i>t</i> ≤ 100</span>) — amount of balls and duration of the process. Then follow <span class="tex-span"><i>n</i></span> lines, each containing three integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>v</i><sub class="lower-index"><i>i</i></sub>|, <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 100, |<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 100</span>) — coordinate, speed and weight of the ball with index <span class="tex-span"><i>i</i></span> at time moment <span class="tex-span">0</span>.</p><p>It is guaranteed that no two balls have the same coordinate initially. Also each collision will be a collision of not more than two balls (that is, three or more balls never collide at the same point in all times from segment <span class="tex-span">[0;<i>t</i>]</span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> numbers — coordinates of the balls <span class="tex-span"><i>t</i></span> seconds after. Output the numbers accurate to at least 4 digits after the decimal point.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10, 0 ≤ <i>t</i> ≤ 100</span>) — amount of balls and duration of the process. Then follow <span class="tex-span"><i>n</i></span> lines, each containing three integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>v</i><sub class="lower-index"><i>i</i></sub>|, <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 100, |<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 100</span>) — coordinate, speed and weight of the ball with index <span class="tex-span"><i>i</i></span> at time moment <span class="tex-span">0</span>.</p><p>It is guaranteed that no two balls have the same coordinate initially. Also each collision will be a collision of not more than two balls (that is, three or more balls never collide at the same point in all times from segment <span class="tex-span">[0;<i>t</i>]</span>).</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> numbers — coordinates of the balls <span class="tex-span"><i>t</i></span> seconds after. Output the numbers accurate to at least 4 digits after the decimal point.</p>





```input1
2 9
3 4 5
0 7 8

```




```input2
3 10
1 2 3
4 -5 6
7 -8 9

```




```output1
68.538461538
44.538461538

```




```output2
-93.666666667
-74.666666667
-15.666666667

```


