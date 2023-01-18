## Description

<div><p>Johnny drives a truck and must deliver a package from his hometown to the district center. His hometown is located at point <span class="tex-span">0</span> on a number line, and the district center is located at the point <span class="tex-span"><i>d</i></span>.</p><p>Johnny's truck has a gas tank that holds exactly <span class="tex-span"><i>n</i></span> liters, and his tank is initially full. As he drives, the truck consumes exactly one liter per unit distance traveled. Moreover, there are <span class="tex-span"><i>m</i></span> gas stations located at various points along the way to the district center. The <span class="tex-span"><i>i</i></span>-th station is located at the point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> on the number line and sells an unlimited amount of fuel at a price of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> dollars per liter. Find the minimum cost Johnny must pay for fuel to successfully complete the delivery.</p></div><div class="input-specification"><p>The first line of input contains three space separated integers <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>n</i></span>, and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the total distance to the district center, the volume of the gas tank, and the number of gas stations, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i> - 1</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the position and cost of gas at the <span class="tex-span"><i>i</i></span>-th gas station. It is guaranteed that the positions of the gas stations are distinct.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum cost to complete the delivery. If there is no way to complete the delivery, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of input contains three space separated integers <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>n</i></span>, and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the total distance to the district center, the volume of the gas tank, and the number of gas stations, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i> - 1</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the position and cost of gas at the <span class="tex-span"><i>i</i></span>-th gas station. It is guaranteed that the positions of the gas stations are distinct.</p>

## Output

<p>Print a single integer&nbsp;— the minimum cost to complete the delivery. If there is no way to complete the delivery, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
10 4 4
3 5
5 8
6 3
8 4

```




```input2
16 5 2
8 2
5 1

```




```output1
22

```




```output2
-1

```



## Note

<p>In the first sample, Johnny's truck holds <span class="tex-span">4</span> liters. He can drive <span class="tex-span">3</span> units to the first gas station, buy <span class="tex-span">2</span> liters of gas there (bringing the tank to <span class="tex-span">3</span> liters total), drive <span class="tex-span">3</span> more units to the third gas station, buy <span class="tex-span">4</span> liters there to fill up his tank, and then drive straight to the district center. His total cost is <span class="tex-span">2·5 + 4·3 = 22</span> dollars.</p><p>In the second sample, there is no way for Johnny to make it to the district center, as his tank cannot hold enough gas to take him from the latest gas station to the district center.</p>
