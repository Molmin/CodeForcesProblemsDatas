## Description

<div><p>Heidi has finally found the mythical Tree of Life – a legendary combinatorial structure which is said to contain a prophecy crucially needed to defeat the undead armies.</p><p>On the surface, the Tree of Life is just a regular undirected tree well-known from computer science. This means that it is a collection of <span class="tex-span"><i>n</i></span> points (called vertices), some of which are connected using <span class="tex-span"><i>n</i> - 1</span> line segments (edges) so that each pair of vertices is connected by a <span class="tex-font-style-it">path</span> (a sequence of one or more edges).</p><p>To decipher the prophecy, Heidi needs to perform a number of steps. The first is counting the number of <span class="tex-font-style-it">lifelines</span> in the tree – these are paths of length <span class="tex-span">2</span>, i.e., consisting of two edges. Help her!</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> – the number of vertices in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). The vertices are labeled with the numbers from 1 to <span class="tex-span"><i>n</i></span>. Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each describing one edge using two space-separated numbers <span class="tex-span"><i>a</i> <i>b</i></span> – the labels of the vertices connected by the edge (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ <i>n</i></span>). It is guaranteed that the input represents a tree.</p></div><div class="output-specification"><p>Print one integer – the number of lifelines in the tree.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> – the number of vertices in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). The vertices are labeled with the numbers from 1 to <span class="tex-span"><i>n</i></span>. Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each describing one edge using two space-separated numbers <span class="tex-span"><i>a</i> <i>b</i></span> – the labels of the vertices connected by the edge (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ <i>n</i></span>). It is guaranteed that the input represents a tree.</p>

## Output

<p>Print one integer – the number of lifelines in the tree.</p>





```input1
4
1 2
1 3
1 4

```




```input2
5
1 2
2 3
3 4
3 5

```




```output1
3
```




```output2
4
```



## Note

<p>In the second sample, there are four lifelines: paths between vertices <span class="tex-span">1</span> and <span class="tex-span">3</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>, <span class="tex-span">2</span> and <span class="tex-span">5</span>, and <span class="tex-span">4</span> and <span class="tex-span">5</span>.</p>
