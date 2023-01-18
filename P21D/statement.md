## Description

<div><p>You are given undirected weighted graph. Find the length of the shortest cycle which starts from the vertex 1 and passes throught all the edges at least once. Graph may contain multiply edges between a pair of vertices and loops (edges from the vertex to itself).</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15, 0 ≤ <i>m</i> ≤ 2000</span>), <span class="tex-span"><i>n</i></span> is the amount of vertices, and <span class="tex-span"><i>m</i></span> is the amount of edges. Following <span class="tex-span"><i>m</i></span> lines contain edges as a triples <span class="tex-span"><i>x</i>, <i>y</i>, <i>w</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10000</span>), <span class="tex-span"><i>x</i>, <i>y</i></span> are edge endpoints, and <span class="tex-span"><i>w</i></span> is the edge length.</p></div><div class="output-specification"><p>Output minimal cycle length or <span class="tex-font-style-tt">-1</span> if it doesn't exists.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15, 0 ≤ <i>m</i> ≤ 2000</span>), <span class="tex-span"><i>n</i></span> is the amount of vertices, and <span class="tex-span"><i>m</i></span> is the amount of edges. Following <span class="tex-span"><i>m</i></span> lines contain edges as a triples <span class="tex-span"><i>x</i>, <i>y</i>, <i>w</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10000</span>), <span class="tex-span"><i>x</i>, <i>y</i></span> are edge endpoints, and <span class="tex-span"><i>w</i></span> is the edge length.</p>

## Output

<p>Output minimal cycle length or <span class="tex-font-style-tt">-1</span> if it doesn't exists.</p>





```input1
3 3
1 2 1
2 3 1
3 1 1

```




```input2
3 2
1 2 3
2 3 4

```




```output1
3

```




```output2
14

```


