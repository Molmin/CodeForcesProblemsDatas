## Description

<div><p>Bessie and the cows have recently been playing with "cool" sequences and are trying to construct some. Unfortunately they are bad at arithmetic, so they need your help!</p><p>A pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of positive integers is "cool" if <span class="tex-span"><i>x</i></span> can be expressed as the sum of <span class="tex-span"><i>y</i></span> consecutive integers (not necessarily positive). A sequence <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> is "cool" if the pairs <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>), (<i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>), ..., (<i>a</i><sub class="lower-index"><i>n</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> are all cool. </p><p>The cows have a sequence of <span class="tex-span"><i>n</i></span> positive integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. In one move, they may replace some <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> with any other positive integer (there are no other limits on the new value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). Determine the smallest number of moves needed to make the resulting sequence cool.</p></div><div class="input-specification"><p>The first line contains a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>A single integer, the minimum number of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> that must be changed to make the sequence cool.</p></div>

## Input

<p>The first line contains a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>A single integer, the minimum number of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> that must be changed to make the sequence cool.</p>





```input1
3
6 4 1

```




```input2
4
20 6 3 4

```




```output1
0

```




```output2
2

```



## Note

<p>In the first sample, the sequence is already cool, so we don't need to change any elements. In the second sample, we can change <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> to 5 and <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> to 10 to make (20, 5, 10, 4) which is cool. This changes 2 elements.</p>
