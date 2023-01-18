## Description

<div><p>Connected undirected graph without cycles is called a tree. Trees is a class of graphs which is interesting not only for people, but for ants too.</p><p>An ant stands at the root of some tree. He sees that there are <span class="tex-span"><i>n</i></span> vertexes in the tree, and they are connected by <span class="tex-span"><i>n</i> - 1</span> edges so that there is a path between any pair of vertexes. A leaf is a distinct from root vertex, which is connected with exactly one other vertex.</p><p>The ant wants to visit every vertex in the tree and return to the root, passing every edge twice. In addition, he wants to visit the leaves in a specific order. You are to find some possible route of the ant.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>) — amount of vertexes in the tree. Next <span class="tex-span"><i>n</i> - 1</span> lines describe edges. Each edge is described with two integers — indexes of vertexes which it connects. Each edge can be passed in any direction. Vertexes are numbered starting from <span class="tex-span">1</span>. The root of the tree has number <span class="tex-span">1</span>. The last line contains <span class="tex-span"><i>k</i></span> integers, where <span class="tex-span"><i>k</i></span> is amount of leaves in the tree. These numbers describe the order in which the leaves should be visited. It is guaranteed that each leaf appears in this order exactly once.</p></div><div class="output-specification"><p>If the required route doesn't exist, output <span class="tex-font-style-tt">-1</span>. Otherwise, output <span class="tex-span">2<i>n</i> - 1</span> numbers, describing the route. Every time the ant comes to a vertex, output it's index.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>) — amount of vertexes in the tree. Next <span class="tex-span"><i>n</i> - 1</span> lines describe edges. Each edge is described with two integers — indexes of vertexes which it connects. Each edge can be passed in any direction. Vertexes are numbered starting from <span class="tex-span">1</span>. The root of the tree has number <span class="tex-span">1</span>. The last line contains <span class="tex-span"><i>k</i></span> integers, where <span class="tex-span"><i>k</i></span> is amount of leaves in the tree. These numbers describe the order in which the leaves should be visited. It is guaranteed that each leaf appears in this order exactly once.</p>

## Output

<p>If the required route doesn't exist, output <span class="tex-font-style-tt">-1</span>. Otherwise, output <span class="tex-span">2<i>n</i> - 1</span> numbers, describing the route. Every time the ant comes to a vertex, output it's index.</p>





```input1
3
1 2
2 3
3

```




```input2
6
1 2
1 3
2 4
4 5
4 6
5 6 3

```




```input3
6
1 2
1 3
2 4
4 5
4 6
5 3 6

```




```output1
1 2 3 2 1
```




```output2
1 2 4 5 4 6 4 2 1 3 1
```




```output3
-1

```


