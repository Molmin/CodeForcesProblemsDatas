## Description

<div><p>You are given a weighted undirected graph on <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. Find the shortest path from vertex <span class="tex-span"><i>s</i></span> to vertex <span class="tex-span"><i>t</i></span> or else state that such path doesn't exist.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the graph edges. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). <span class="tex-font-style-bf">That means that vertices with numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> are connected by edge of length <span class="tex-span">2<sup class="upper-index"><i>x</i><sub class="lower-index"><i>i</i></sub></sup></span> (2 to the power of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>).</span></p><p>The last line contains two space-separated integers — the numbers of vertices <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p><p>The vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The graph contains no multiple edges and self-loops.</p></div><div class="output-specification"><p>In the first line print the remainder after dividing the length of the shortest path by <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span> if the path exists, and <span class="tex-font-style-tt">-1</span> if the path doesn't exist.</p><p>If the path exists print in the second line integer <span class="tex-span"><i>k</i></span> — the number of vertices in the shortest path from vertex <span class="tex-span"><i>s</i></span> to vertex <span class="tex-span"><i>t</i></span>; in the third line print <span class="tex-span"><i>k</i></span> space-separated integers — the vertices of the shortest path in the visiting order. The first vertex should be vertex <span class="tex-span"><i>s</i></span>, the last vertex should be vertex <span class="tex-span"><i>t</i></span>. If there are multiple shortest paths, print any of them.</p></div>

## Input

<p>The first line of the input contains two space-separated integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the graph edges. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). <span class="tex-font-style-bf">That means that vertices with numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> are connected by edge of length <span class="tex-span">2<sup class="upper-index"><i>x</i><sub class="lower-index"><i>i</i></sub></sup></span> (2 to the power of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>).</span></p><p>The last line contains two space-separated integers — the numbers of vertices <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p><p>The vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The graph contains no multiple edges and self-loops.</p>

## Output

<p>In the first line print the remainder after dividing the length of the shortest path by <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span> if the path exists, and <span class="tex-font-style-tt">-1</span> if the path doesn't exist.</p><p>If the path exists print in the second line integer <span class="tex-span"><i>k</i></span> — the number of vertices in the shortest path from vertex <span class="tex-span"><i>s</i></span> to vertex <span class="tex-span"><i>t</i></span>; in the third line print <span class="tex-span"><i>k</i></span> space-separated integers — the vertices of the shortest path in the visiting order. The first vertex should be vertex <span class="tex-span"><i>s</i></span>, the last vertex should be vertex <span class="tex-span"><i>t</i></span>. If there are multiple shortest paths, print any of them.</p>





```input1
4 4
1 4 2
1 2 0
2 3 0
3 4 0
1 4

```




```input2
4 3
1 2 4
2 3 5
3 4 6
1 4

```




```input3
4 2
1 2 0
3 4 1
1 4

```




```output1
3
4
1 2 3 4 

```




```output2
112
4
1 2 3 4 

```




```output3
-1

```



## Note

<p>A <span class="tex-font-style-underline">path</span> from vertex <span class="tex-span"><i>s</i></span> to vertex <span class="tex-span"><i>t</i></span> is a sequence <span class="tex-span"><i>v</i><sub class="lower-index">0</sub></span>, ..., <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span>, such that <span class="tex-span"><i>v</i><sub class="lower-index">0</sub> = <i>s</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub> = <i>t</i></span>, and for any <span class="tex-span"><i>i</i></span> from 0 to <span class="tex-span"><i>k</i> - 1</span> vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> are connected by an edge. </p><p>The <span class="tex-font-style-underline">length</span> of the path is the sum of weights of edges between <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from 0 to <span class="tex-span"><i>k</i> - 1</span>. </p><p>The <span class="tex-font-style-underline">shortest path</span> from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span> is the path which length is minimum among all possible paths from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>.</p>
