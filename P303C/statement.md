## Description

<div><p>You have been given <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You can remove at most <span class="tex-span"><i>k</i></span> of them. Find the minimum modular <span class="tex-span"><i>m</i></span> <span class="tex-span">(<i>m</i> &gt; 0)</span>, so that for every pair of the remaining integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span>, the following unequality holds: <img align="middle" class="tex-formula" src="file://acY4g3cs.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1  ≤ <i>n</i>  ≤ 5000, 0 ≤ <i>k</i> ≤ 4</span>), which we have mentioned above. </p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>Print a single positive integer — the minimum <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1  ≤ <i>n</i>  ≤ 5000, 0 ≤ <i>k</i> ≤ 4</span>), which we have mentioned above. </p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>Print a single positive integer — the minimum <span class="tex-span"><i>m</i></span>.</p>





```input1
7 0
0 2 3 6 7 12 18

```




```input2
7 1
0 2 3 6 7 12 18

```




```output1
13

```




```output2
7

```


