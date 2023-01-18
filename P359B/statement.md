## Description

<div><p>A <span class="tex-font-style-it">permutation</span> <span class="tex-span"><i>p</i></span> is an ordered group of numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,   <i>p</i><sub class="lower-index">2</sub>,   ...,   <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each is no more than <span class="tex-span"><i>n</i></span>. We'll define number <span class="tex-span"><i>n</i></span> as the length of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,   <i>p</i><sub class="lower-index">2</sub>,   ...,   <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Simon has a positive integer <span class="tex-span"><i>n</i></span> and a non-negative integer <span class="tex-span"><i>k</i></span>, such that <span class="tex-span">2<i>k</i> ≤ <i>n</i></span>. Help him find permutation <span class="tex-span"><i>a</i></span> of length <span class="tex-span">2<i>n</i></span>, such that it meets this equation: <img align="middle" class="tex-formula" src="file://BBUuEQEz.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>, <span class="tex-span">0 ≤ 2<i>k</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span">2<i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<i>n</i></sub></span> — the required permutation <span class="tex-span"><i>a</i></span>. It is guaranteed that the solution exists. If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>, <span class="tex-span">0 ≤ 2<i>k</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print <span class="tex-span">2<i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<i>n</i></sub></span> — the required permutation <span class="tex-span"><i>a</i></span>. It is guaranteed that the solution exists. If there are multiple solutions, you can print any of them.</p>





```input1
1 0

```




```input2
2 1

```




```input3
4 0

```




```output1
1 2
```




```output2
3 2 1 4

```




```output3
2 7 4 6 1 3 5 8

```



## Note

<p>Record <span class="tex-span">|<i>x</i>|</span> represents the absolute value of number <span class="tex-span"><i>x</i></span>. </p><p>In the first sample <span class="tex-span">|1 - 2| - |1 - 2| = 0</span>.</p><p>In the second sample <span class="tex-span">|3 - 2| + |1 - 4| - |3 - 2 + 1 - 4| = 1 + 3 - 2 = 2</span>.</p><p>In the third sample <span class="tex-span">|2 - 7| + |4 - 6| + |1 - 3| + |5 - 8| - |2 - 7 + 4 - 6 + 1 - 3 + 5 - 8| = 12 - 12 = 0</span>.</p>
