## Description

<div><p>You've got a weighted tree, consisting of <span class="tex-span"><i>n</i></span> vertices. Each edge has a non-negative weight. The length of the path between any two vertices of the tree is the number of edges in the path. The weight of the path is the total weight of all edges it contains. </p><p>Two vertices are close if there exists a path of length at most <span class="tex-span"><i>l</i></span> between them and a path of weight at most <span class="tex-span"><i>w</i></span> between them. Count the number of pairs of vertices <span class="tex-span"><i>v</i>, <i>u</i></span> <span class="tex-span">(<i>v</i> &lt; <i>u</i>)</span>, such that vertices <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> are close.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>l</i> ≤ <i>n</i>, 0 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The next <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of the tree edges. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; (<i>i</i> + 1), 0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>, that mean that the <span class="tex-span"><i>i</i></span>-th edge connects vertex <span class="tex-span">(<i>i</i> + 1)</span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and has weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider the tree vertices indexed from 1 to <span class="tex-span"><i>n</i></span> in some way.</p></div><div class="output-specification"><p>Print a single integer — the number of close pairs.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>l</i> ≤ <i>n</i>, 0 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The next <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of the tree edges. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; (<i>i</i> + 1), 0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>, that mean that the <span class="tex-span"><i>i</i></span>-th edge connects vertex <span class="tex-span">(<i>i</i> + 1)</span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and has weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider the tree vertices indexed from 1 to <span class="tex-span"><i>n</i></span> in some way.</p>

## Output

<p>Print a single integer — the number of close pairs.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4 4 6
1 3
1 4
1 3

```




```input2
6 2 17
1 3
2 5
2 13
1 6
5 9

```




```output1
4

```




```output2
9

```


