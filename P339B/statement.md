## Description

<div><p>Xenia lives in a city that has <span class="tex-span"><i>n</i></span> houses built along the main ringroad. The ringroad houses are numbered 1 through <span class="tex-span"><i>n</i></span> in the clockwise order. The ringroad traffic is one way and also is clockwise.</p><p>Xenia has recently moved into the ringroad house number 1. As a result, she's got <span class="tex-span"><i>m</i></span> things to do. In order to complete the <span class="tex-span"><i>i</i></span>-th task, she needs to be in the house number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and complete all tasks with numbers less than <span class="tex-span"><i>i</i></span>. Initially, Xenia is in the house number 1, find the minimum time she needs to complete all her tasks if moving from a house to a neighboring one along the ringroad takes one unit of time.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Note that Xenia can have multiple consecutive tasks in one house.</p></div><div class="output-specification"><p>Print a single integer — the time Xenia needs to complete all tasks.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Note that Xenia can have multiple consecutive tasks in one house.</p>

## Output

<p>Print a single integer — the time Xenia needs to complete all tasks.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4 3
3 2 3

```




```input2
4 3
2 3 3

```




```output1
6

```




```output2
2

```



## Note

<p>In the first test example the sequence of Xenia's moves along the ringroad looks as follows: <span class="tex-span">1 → 2 → 3 → 4 → 1 → 2 → 3</span>. This is optimal sequence. So, she needs 6 time units.</p>
