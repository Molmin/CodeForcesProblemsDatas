## Description

<div><p>Little penguin Polo has got a tree — a non-directed connected acyclic graph, containing <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>n</i> - 1</span> edges. We will consider the tree nodes numbered by integers from 1 to <span class="tex-span"><i>n</i></span>.</p><p>Today Polo wonders, how to find the number of pairs of paths that don't have common nodes. More formally, he should find the number of groups of four integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span> and <span class="tex-span"><i>d</i></span> such that:</p><ul> <li> <span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ <i>n</i></span>; </li><li> <span class="tex-span">1 ≤ <i>c</i> &lt; <i>d</i> ≤ <i>n</i></span>; </li><li> there's no such node that lies on both the shortest path from node <span class="tex-span"><i>a</i></span> to node <span class="tex-span"><i>b</i></span> and from node <span class="tex-span"><i>c</i></span> to node <span class="tex-span"><i>d</i></span>. </li></ul><p>The shortest path betweem two nodes is the path that is shortest in the number of edges.</p><p>Help Polo solve this problem.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 80000)</span> — the number of tree nodes. Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> — the <span class="tex-span"><i>i</i></span>-th edge of the tree.</p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is recommended to use the cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 80000)</span> — the number of tree nodes. Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> — the <span class="tex-span"><i>i</i></span>-th edge of the tree.</p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is recommended to use the cin, cout streams or the %I64d specificator.</p>





```input1
4
1 2
2 3
3 4

```




```output1
2

```


