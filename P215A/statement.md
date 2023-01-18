## Description

<div><p>Vasya's bicycle chain drive consists of two parts: <span class="tex-span"><i>n</i></span> stars are attached to the pedal axle, <span class="tex-span"><i>m</i></span> stars are attached to the rear wheel axle. The chain helps to rotate the rear wheel by transmitting the pedal rotation.</p><p>We know that the <span class="tex-span"><i>i</i></span>-th star on the pedal axle has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 &lt; <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> teeth, and the <span class="tex-span"><i>j</i></span>-th star on the rear wheel axle has <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(0 &lt; <i>b</i><sub class="lower-index">1</sub> &lt; <i>b</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>b</i><sub class="lower-index"><i>m</i></sub>)</span> teeth. Any pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i></span>;&nbsp;<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i>)</span> is called a <span class="tex-font-style-it">gear</span> and sets the indexes of stars to which the chain is currently attached. Gear <span class="tex-span">(<i>i</i>, <i>j</i>)</span> has a gear ratio, equal to the value <img align="middle" class="tex-formula" src="file://jGeXWiUm.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Since Vasya likes integers, he wants to find such gears <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, that their ratios are integers. On the other hand, Vasya likes fast driving, so among all "integer" gears <span class="tex-span">(<i>i</i>, <i>j</i>)</span> he wants to choose a gear with the maximum ratio. Help him to find the number of such gears.</p><p>In the problem, fraction <img align="middle" class="tex-formula" src="file://VKEIMekp.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes division in real numbers, that is, no rounding is performed.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the number of stars on the bicycle's pedal axle. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> in the order of strict increasing.</p><p>The third input line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 50)</span> — the number of stars on the rear wheel axle. The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> in the order of strict increasing.</p><p>It is guaranteed that there exists at least one gear (<span class="tex-span"><i>i</i>, <i>j</i></span>), that its gear ratio is an integer. The numbers on the lines are separated by spaces.</p></div><div class="output-specification"><p>Print the number of "integer" gears with the maximum ratio among all "integer" gears.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the number of stars on the bicycle's pedal axle. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> in the order of strict increasing.</p><p>The third input line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 50)</span> — the number of stars on the rear wheel axle. The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> in the order of strict increasing.</p><p>It is guaranteed that there exists at least one gear (<span class="tex-span"><i>i</i>, <i>j</i></span>), that its gear ratio is an integer. The numbers on the lines are separated by spaces.</p>

## Output

<p>Print the number of "integer" gears with the maximum ratio among all "integer" gears.</p>





```input1
2
4 5
3
12 13 15

```




```input2
4
1 2 3 4
5
10 11 12 13 14

```




```output1
2

```




```output2
1

```



## Note

<p>In the first sample the maximum "integer" gear ratio equals 3. There are two gears that have such gear ratio. For one of them <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 4, <i>b</i><sub class="lower-index">1</sub> = 12</span>, and for the other <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 5, <i>b</i><sub class="lower-index">3</sub> = 15</span>.</p>
