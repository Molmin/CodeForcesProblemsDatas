## Description

<div><p>Everyone knows what the Fibonacci sequence is. This sequence can be defined by the recurrence relation: </p><center class="tex-equation"><span class="tex-span"><i>F</i><sub class="lower-index">1</sub> = 1, <i>F</i><sub class="lower-index">2</sub> = 2, <i>F</i><sub class="lower-index"><i>i</i></sub> = <i>F</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>F</i><sub class="lower-index"><i>i</i> - 2</sub>&nbsp;(<i>i</i> &gt; 2).</span></center><p>We'll define a new number sequence <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub>(<i>k</i>)</span> by the formula: </p><center class="tex-equation"><span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub>(<i>k</i>) = <i>F</i><sub class="lower-index"><i>i</i></sub> × <i>i</i><sup class="upper-index"><i>k</i></sup>&nbsp;(<i>i</i> ≥ 1).</span></center><p>In this problem, your task is to calculate the following sum: <span class="tex-span"><i>A</i><sub class="lower-index">1</sub>(<i>k</i>) + <i>A</i><sub class="lower-index">2</sub>(<i>k</i>) + ... + <i>A</i><sub class="lower-index"><i>n</i></sub>(<i>k</i>)</span>. The answer can be very large, so print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">17</sup>;&nbsp;1 ≤ <i>k</i> ≤ 40)</span>.</p></div><div class="output-specification"><p>Print a single integer — the sum of the first <span class="tex-span"><i>n</i></span> elements of the sequence <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub>(<i>k</i>)</span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">17</sup>;&nbsp;1 ≤ <i>k</i> ≤ 40)</span>.</p>

## Output

<p>Print a single integer — the sum of the first <span class="tex-span"><i>n</i></span> elements of the sequence <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub>(<i>k</i>)</span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 1

```




```input2
4 1

```




```input3
5 2

```




```input4
7 4

```




```output1
1

```




```output2
34

```




```output3
316

```




```output4
73825

```


