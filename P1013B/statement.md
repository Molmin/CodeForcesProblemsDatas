## Description

<div><p>There is an array with <span class="tex-span"><i>n</i></span> elements <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and the number <span class="tex-span"><i>x</i></span>.</p><p>In one operation you can select some <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) and replace element <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &amp; <i>x</i></span>, where <span class="tex-span">&amp;</span> denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise and</a> operation.</p><p>You want the array to have at least two equal elements after applying some operations (possibly, none). In other words, there should be at least two distinct indices <span class="tex-span"><i>i</i> ≠ <i>j</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub></span>. Determine whether it is possible to achieve and, if possible, the minimal number of operations to apply.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 100 000</span>), number of elements in the array and the number to and with.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), the elements of the array.</p></div><div class="output-specification"><p>Print a single integer denoting the minimal number of operations to do, or <span class="tex-font-style-tt">-1</span>, if it is impossible.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 100 000</span>), number of elements in the array and the number to and with.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), the elements of the array.</p>

## Output

<p>Print a single integer denoting the minimal number of operations to do, or <span class="tex-font-style-tt">-1</span>, if it is impossible.</p>





```input1
4 3
1 2 3 7

```




```input2
2 228
1 1

```




```input3
3 7
1 2 3

```




```output1
1

```




```output2
0

```




```output3
-1

```



## Note

<p>In the first example one can apply the operation to the last element of the array. That replaces 7 with 3, so we achieve the goal in one move.</p><p>In the second example the array already has two equal elements.</p><p>In the third example applying the operation won't change the array at all, so it is impossible to make some pair of elements equal.</p>
