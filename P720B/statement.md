## Description

<div><p>Tree is a connected undirected graph that has no cycles. Edge cactus is a connected undirected graph without loops and parallel edges, such that each edge belongs to at most one cycle.</p><p>Vasya has an edge cactus, each edge of this graph has some color.</p><p>Vasya would like to remove the minimal number of edges in such way that his cactus turned to a tree. Vasya wants to make it in such a way that there were edges of as many different colors in the resulting tree, as possible. Help him to find how many different colors can the resulting tree have.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10 000</span>)&nbsp;— the number of vertices and the number of edges in Vasya's graph, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain three integers each: <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>)&nbsp;— the numbers of vertices connected by the corresponding edge, and its color. It is guaranteed that the described graph is indeed an edge cactus.</p></div><div class="output-specification"><p>Output one integer: the maximal number of different colors that the resulting tree can have.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10 000</span>)&nbsp;— the number of vertices and the number of edges in Vasya's graph, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain three integers each: <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>)&nbsp;— the numbers of vertices connected by the corresponding edge, and its color. It is guaranteed that the described graph is indeed an edge cactus.</p>

## Output

<p>Output one integer: the maximal number of different colors that the resulting tree can have.</p>





```input1
4 4
1 2 4
2 3 1
3 4 2
4 2 3

```




```input2
7 9
1 2 1
2 3 4
3 1 5
1 4 5
4 5 2
5 1 6
1 6 4
6 7 6
7 1 3

```




```output1
3

```




```output2
6

```


