## Description

<div><p>The winter in Berland lasts <span class="tex-span"><i>n</i></span> days. For each day we know the forecast for the average air temperature that day. </p><p>Vasya has a new set of winter tires which allows him to drive safely no more than <span class="tex-span"><i>k</i></span> days at any average air temperature. After <span class="tex-span"><i>k</i></span> days of using it (regardless of the temperature of these days) the set of winter tires wears down and cannot be used more. It is not necessary that these <span class="tex-span"><i>k</i></span> days form a continuous segment of days.</p><p>Before the first winter day Vasya still uses <span class="tex-font-style-bf">summer tires</span>. It is possible to drive safely on summer tires any number of days when the average air temperature is <span class="tex-font-style-bf">non-negative</span>. It is impossible to drive on summer tires at days when the average air temperature is negative. </p><p>Vasya can change summer tires to winter tires and vice versa at the beginning of any day.</p><p>Find the minimum number of times Vasya needs to change summer tires to winter tires and vice versa to drive safely during the winter. At the end of the winter the car can be with any set of tires.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of winter days and the number of days winter tires can be used. It is allowed to drive on winter tires at any temperature, but no more than <span class="tex-span"><i>k</i></span> days in total.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 20 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>)&nbsp;— the average air temperature in the <span class="tex-span"><i>i</i></span>-th winter day. </p></div><div class="output-specification"><p>Print the minimum number of times Vasya has to change summer tires to winter tires and vice versa to drive safely during all winter. If it is impossible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of winter days and the number of days winter tires can be used. It is allowed to drive on winter tires at any temperature, but no more than <span class="tex-span"><i>k</i></span> days in total.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 20 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>)&nbsp;— the average air temperature in the <span class="tex-span"><i>i</i></span>-th winter day. </p>

## Output

<p>Print the minimum number of times Vasya has to change summer tires to winter tires and vice versa to drive safely during all winter. If it is impossible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 3
-5 20 -3 0

```




```input2
4 2
-5 20 -3 0

```




```input3
10 6
2 -5 1 3 0 0 -4 -3 1 0

```




```output1
2

```




```output2
4

```




```output3
3

```



## Note

<p>In the first example before the first winter day Vasya should change summer tires to winter tires, use it for three days, and then change winter tires to summer tires because he can drive safely with the winter tires for just three days. Thus, the total number of tires' changes equals two. </p><p>In the second example before the first winter day Vasya should change summer tires to winter tires, and then after the first winter day change winter tires to summer tires. After the second day it is necessary to change summer tires to winter tires again, and after the third day it is necessary to change winter tires to summer tires. Thus, the total number of tires' changes equals four. </p>
