## Description

<div><p>Valera has <span class="tex-span"><i>n</i></span> counters numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some of them are connected by wires, and each of the counters has a special button.</p><p>Initially, all the counters contain number <span class="tex-span">0</span>. When you press a button on a certain counter, the value it has increases by one. Also, the values recorded in all the counters, directly connected to it by a wire, increase by one.</p><p>Valera and Ignat started having a dispute, the dispute is as follows. Ignat thought of a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Valera should choose some set of distinct counters and press buttons on each of them exactly once (on other counters the buttons won't be pressed). If after that there is a counter with the number <span class="tex-span"><i>i</i></span>, which has value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, then Valera loses the dispute, otherwise he wins the dispute.</p><p>Help Valera to determine on which counters he needs to press a button to win the dispute.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>, that denote the number of counters Valera has and the number of pairs of counters connected by wires.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>, that mean that counters with numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> are connected by a wire. It is guaranteed that each pair of connected counters occurs exactly once in the input.</p><p>The last line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the value that Ignat choose for the <span class="tex-span"><i>i</i></span>-th counter.</p></div><div class="output-specification"><p>If Valera can't win the dispute print in the first line -1.</p><p>Otherwise, print in the first line integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ <i>n</i>)</span>. In the second line print <span class="tex-span"><i>k</i></span> distinct space-separated integers — the numbers of the counters, where Valera should push buttons to win the dispute, in arbitrary order.</p><p>If there exists multiple answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>, that denote the number of counters Valera has and the number of pairs of counters connected by wires.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>, that mean that counters with numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> are connected by a wire. It is guaranteed that each pair of connected counters occurs exactly once in the input.</p><p>The last line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the value that Ignat choose for the <span class="tex-span"><i>i</i></span>-th counter.</p>

## Output

<p>If Valera can't win the dispute print in the first line -1.</p><p>Otherwise, print in the first line integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ <i>n</i>)</span>. In the second line print <span class="tex-span"><i>k</i></span> distinct space-separated integers — the numbers of the counters, where Valera should push buttons to win the dispute, in arbitrary order.</p><p>If there exists multiple answers, you are allowed to print any of them.</p>





```input1
5 5
2 3
4 1
1 5
5 3
2 1
1 1 2 0 2

```




```input2
4 2
1 2
3 4
0 0 0 0

```




```output1
2
1 2

```




```output2
3
1 3 4

```


