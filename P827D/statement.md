## Description

<div><p>You are given a connected weighted graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. The graph doesn't contain loops nor multiple edges. Consider some edge with id <span class="tex-span"><i>i</i></span>. Let's determine for this edge the maximum integer weight we can give to it so that it is contained in all minimum spanning trees of the graph if we don't change the other weights.</p><p>You are to determine this maximum weight described above for each edge. You should calculate the answer for each edge independently, it means there can't be two edges with changed weights at the same time.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are the number of vertices and the number of edges in the graph, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>) meaning that there is an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> with weight <span class="tex-span"><i>c</i></span>. </p></div><div class="output-specification"><p>Print the answer for each edge in the order the edges are given in the input. If an edge is contained in every minimum spanning tree with any weight, print <span class="tex-font-style-tt">-1</span> as the answer.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are the number of vertices and the number of edges in the graph, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>) meaning that there is an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> with weight <span class="tex-span"><i>c</i></span>. </p>

## Output

<p>Print the answer for each edge in the order the edges are given in the input. If an edge is contained in every minimum spanning tree with any weight, print <span class="tex-font-style-tt">-1</span> as the answer.</p>





```input1
4 4
1 2 2
2 3 2
3 4 2
4 1 3

```




```input2
4 3
1 2 2
2 3 2
3 4 2

```




```output1
2 2 2 1
```




```output2
-1 -1 -1
```


