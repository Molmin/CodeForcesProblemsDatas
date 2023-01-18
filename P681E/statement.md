## Description

<div><p>Dima is living in a dormitory, as well as some cockroaches.</p><p>At the moment <span class="tex-span">0</span> Dima saw a cockroach running on a table and decided to kill it. Dima needs exactly <span class="tex-span"><i>T</i></span> seconds for aiming, and after that he will precisely strike the cockroach and finish it.</p><p>To survive the cockroach has to run into a shadow, cast by round plates standing on the table, in <span class="tex-span"><i>T</i></span> seconds. Shadow casted by any of the plates has the shape of a circle. Shadow circles may intersect, nest or overlap arbitrarily.</p><p>The cockroach uses the following strategy: first he equiprobably picks a direction to run towards and then runs towards it with the constant speed <span class="tex-span"><i>v</i></span>. If at some moment <span class="tex-span"><i>t</i> ≤ <i>T</i></span> it reaches any shadow circle, it immediately stops in the shadow and thus will stay alive. Otherwise the cockroach is killed by the Dima's precise strike. Consider that the Dima's precise strike is instant.</p><p>Determine the probability of that the cockroach will stay alive.</p></div><div class="input-specification"><p>In the first line of the input the four integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>T</i></span> (<span class="tex-span">|<i>x</i><sub class="lower-index">0</sub>|, |<i>y</i><sub class="lower-index">0</sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>v</i>, <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>) are given&nbsp;— the cockroach initial position on the table in the Cartesian system at the moment <span class="tex-span">0</span>, the cockroach's constant speed and the time in seconds Dima needs for aiming respectively.</p><p>In the next line the only number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) is given&nbsp;— the number of shadow circles casted by plates.</p><p>In the next <span class="tex-span"><i>n</i></span> lines shadow circle description is given: the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them consists of three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> shadow circle on-table position in the Cartesian system and its radius respectively.</p><p>Consider that the table is big enough for the cockroach not to run to the table edges and avoid Dima's precise strike.</p></div><div class="output-specification"><p>Print the only real number <span class="tex-span"><i>p</i></span>&nbsp;— the probability of that the cockroach will stay alive.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>In the first line of the input the four integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>T</i></span> (<span class="tex-span">|<i>x</i><sub class="lower-index">0</sub>|, |<i>y</i><sub class="lower-index">0</sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>v</i>, <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>) are given&nbsp;— the cockroach initial position on the table in the Cartesian system at the moment <span class="tex-span">0</span>, the cockroach's constant speed and the time in seconds Dima needs for aiming respectively.</p><p>In the next line the only number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) is given&nbsp;— the number of shadow circles casted by plates.</p><p>In the next <span class="tex-span"><i>n</i></span> lines shadow circle description is given: the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them consists of three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> shadow circle on-table position in the Cartesian system and its radius respectively.</p><p>Consider that the table is big enough for the cockroach not to run to the table edges and avoid Dima's precise strike.</p>

## Output

<p>Print the only real number <span class="tex-span"><i>p</i></span>&nbsp;— the probability of that the cockroach will stay alive.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
0 0 1 1
3
1 1 1
-1 -1 1
-2 2 1

```




```input2
0 0 1 0
1
1 0 1

```




```output1
0.50000000000
```




```output2
1.00000000000
```



## Note

<p>The picture for the first sample is given below. </p><center> <img class="tex-graphics" src="file://XRi68Hlu.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Red color stands for points which being chosen as the cockroach's running direction will cause him being killed, green color for those standing for survival directions. Please note that despite containing a circle centered in <span class="tex-span">( - 2, 2)</span> a part of zone is colored red because the cockroach is not able to reach it in one second.</p>
