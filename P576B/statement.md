## Description

<div><p>A tree of size <span class="tex-span"><i>n</i></span> is an undirected connected graph consisting of <span class="tex-span"><i>n</i></span> vertices without cycles.</p><p>Consider some tree with <span class="tex-span"><i>n</i></span> vertices. We call a tree <span class="tex-font-style-it">invariant</span> relative to permutation <span class="tex-span"><i>p</i> = <i>p</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">2</sub>... <i>p</i><sub class="lower-index"><i>n</i></sub></span>, if for any two vertices of the tree <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> the condition holds: "vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are connected by an edge if and only if vertices <span class="tex-span"><i>p</i><sub class="lower-index"><i>u</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>v</i></sub></span> are connected by an edge".</p><p>You are given permutation <span class="tex-span"><i>p</i></span> of size <span class="tex-span"><i>n</i></span>. Find some tree size <span class="tex-span"><i>n</i></span>, invariant relative to the given permutation.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the permutation (also equal to the size of the sought tree).</p><p>The second line contains permutation <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>If the sought tree does not exist, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>", and then print <span class="tex-span"><i>n</i> - 1</span> lines, each of which contains two integers — the numbers of vertices connected by an edge of the tree you found. The vertices are numbered from 1, the order of the edges and the order of the vertices within the edges does not matter.</p><p>If there are multiple solutions, output any of them.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the permutation (also equal to the size of the sought tree).</p><p>The second line contains permutation <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>If the sought tree does not exist, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>", and then print <span class="tex-span"><i>n</i> - 1</span> lines, each of which contains two integers — the numbers of vertices connected by an edge of the tree you found. The vertices are numbered from 1, the order of the edges and the order of the vertices within the edges does not matter.</p><p>If there are multiple solutions, output any of them.</p>





```input1
4
4 3 2 1

```




```input2
3
3 1 2

```




```output1
YES
4 1
4 2
1 3

```




```output2
NO

```



## Note

<p>In the first sample test a permutation transforms edge (4, 1) into edge (1, 4), edge (4, 2) into edge (1, 3) and edge (1, 3) into edge (4, 2). These edges all appear in the resulting tree.</p><p>It can be shown that in the second sample test no tree satisfies the given condition.</p>
