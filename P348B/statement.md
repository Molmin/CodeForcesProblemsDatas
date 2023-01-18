## Description

<div><p>You are given a rooted tree with <span class="tex-span"><i>n</i></span> vertices. In each leaf vertex there's a single integer — the number of apples in this vertex. </p><p>The <span class="tex-font-style-it">weight</span> of a subtree is the sum of all numbers in this subtree leaves. For instance, the weight of a subtree that corresponds to some leaf is the number written in the leaf.</p><p>A tree is <span class="tex-font-style-it">balanced</span> if for every vertex <span class="tex-span"><i>v</i></span> of the tree all its subtrees, corresponding to the children of vertex <span class="tex-span"><i>v</i></span>, are of equal weight. </p><p>Count the minimum number of apples that you need to remove from the tree (specifically, from some of its leaves) in order to make the tree balanced. Notice that you can always achieve the goal by just removing all apples.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing the number of vertices in the tree. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of apples in the vertex number <span class="tex-span"><i>i</i></span>. The number of apples in non-leaf vertices is guaranteed to be zero. </p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines, describing the tree edges. Each line contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>) — the vertices connected by an edge. </p><p>The vertices are indexed from 1 to <span class="tex-span"><i>n</i></span>. Vertex 1 is the root.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of apples to remove in order to make the tree balanced.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the sin, cout streams <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing the number of vertices in the tree. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of apples in the vertex number <span class="tex-span"><i>i</i></span>. The number of apples in non-leaf vertices is guaranteed to be zero. </p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines, describing the tree edges. Each line contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>) — the vertices connected by an edge. </p><p>The vertices are indexed from 1 to <span class="tex-span"><i>n</i></span>. Vertex 1 is the root.</p>

## Output

<p>Print a single integer — the minimum number of apples to remove in order to make the tree balanced.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the sin, cout streams <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
6
0 0 12 13 5 6
1 2
1 3
1 4
2 5
2 6

```




```output1
6
```


