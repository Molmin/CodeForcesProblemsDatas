## Description

<div><p>A root tree is a directed acyclic graph that contains one node (root), from which there is exactly one path to any other node.</p><p>A root tree is binary if each node has at most two outgoing arcs.</p><p>When a binary tree is painted on the plane, all arcs should be directed from top to bottom. That is, each arc going from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> must meet the condition <span class="tex-span"><i>y</i><sub class="lower-index"><i>u</i></sub> &gt; <i>y</i><sub class="lower-index"><i>v</i></sub></span>.</p><p>You've been given the coordinates of all tree nodes. Your task is to connect these nodes by arcs so as to get the binary root tree and make the total length of the arcs minimum. All arcs of the built tree must be directed from top to bottom.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>) — the number of nodes in the tree. Then follow <span class="tex-span"><i>n</i></span> lines, two integers per line: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup></span>) — coordinates of the nodes. It is guaranteed that all points are distinct.</p></div><div class="output-specification"><p>If it is impossible to build a binary root tree on the given points, print "<span class="tex-font-style-tt">-1</span>". Otherwise, print a single real number — the total length of the arcs in the minimum binary tree. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>) — the number of nodes in the tree. Then follow <span class="tex-span"><i>n</i></span> lines, two integers per line: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup></span>) — coordinates of the nodes. It is guaranteed that all points are distinct.</p>

## Output

<p>If it is impossible to build a binary root tree on the given points, print "<span class="tex-font-style-tt">-1</span>". Otherwise, print a single real number — the total length of the arcs in the minimum binary tree. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p>





```input1
3
0 0
1 0
2 1

```




```input2
4
0 0
1 0
2 1
2 0

```




```output1
3.650281539872885

```




```output2
-1

```


