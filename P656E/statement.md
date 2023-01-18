## Description

<div><p>You are given a complete undirected graph. For each pair of vertices you are given the length of the edge that connects them. Find the shortest paths between each pair of vertices in the graph and return the length of the longest of them.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">3 ≤ <i>N</i> ≤ 10</span>).</p><p>The following <span class="tex-span"><i>N</i></span> lines each contain <span class="tex-span"><i>N</i></span> space-separated integers. <span class="tex-span"><i>j</i></span>th integer in <span class="tex-span"><i>i</i></span>th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> is the length of the edge that connects vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = <i>a</i><sub class="lower-index"><i>ji</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>ii</i></sub> = 0</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span> for <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p></div><div class="output-specification"><p>Output the maximum length of the shortest path between any pair of vertices in the graph.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">3 ≤ <i>N</i> ≤ 10</span>).</p><p>The following <span class="tex-span"><i>N</i></span> lines each contain <span class="tex-span"><i>N</i></span> space-separated integers. <span class="tex-span"><i>j</i></span>th integer in <span class="tex-span"><i>i</i></span>th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> is the length of the edge that connects vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = <i>a</i><sub class="lower-index"><i>ji</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>ii</i></sub> = 0</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span> for <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p>

## Output

<p>Output the maximum length of the shortest path between any pair of vertices in the graph.</p>





```input1
3
0 1 1
1 0 4
1 4 0

```




```input2
4
0 1 2 3
1 0 4 5
2 4 0 6
3 5 6 0

```




```output1
2

```




```output2
5

```



## Note

<p>You're running short of keywords, so you can't use some of them:</p><pre class="verbatim">define<br>do<br>for<br>foreach<br>while<br>repeat<br>until<br>if<br>then<br>else<br>elif<br>elsif<br>elseif<br>case<br>switch<br></pre>
