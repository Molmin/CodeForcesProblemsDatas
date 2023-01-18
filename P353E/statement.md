## Description

<div><p>You have a directed acyclic graph <span class="tex-span"><i>G</i></span>, consisting of <span class="tex-span"><i>n</i></span> vertexes, numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. The graph contains <span class="tex-span"><i>n</i></span> edges numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. An edge with number <span class="tex-span"><i>i</i></span> connects vertexes <span class="tex-span"><i>i</i></span> and <span class="tex-span">(<i>i</i> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span>, and it can be directed in either direction (from <span class="tex-span"><i>i</i></span> to <span class="tex-span">(<i>i</i> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span>, or vise versa).</p><p>Operation <span class="tex-span"><i>x</i>&nbsp;<i>mod</i>&nbsp;<i>y</i></span> means taking the remainder after dividing number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>.</p><p>Let's call two vertexes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> in graph <span class="tex-span"><i>G</i></span> comparable if the graph contains a path either from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> or from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>. We'll assume that an antichain is a set of vertexes of graph <span class="tex-span"><i>G</i></span>, where any two distinct vertexes are not comparable. The size of an antichain is the number of vertexes in the corresponding set. An antichain is maximum if the graph doesn't have antichains of a larger size.</p><p>Your task is to find the size of the maximum antichain in graph <span class="tex-span"><i>G</i></span>.</p></div><div class="input-specification"><p>The first line contains the sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">0</sub><i>s</i><sub class="lower-index">1</sub>... <i>s</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, consisting of numbers zero and one. The length of the line (number <span class="tex-span"><i>n</i></span>) corresponds to the number of vertexes and edges in graph <span class="tex-span"><i>G</i></span>. If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>i</i> ≥ 0)</span> equals <span class="tex-span">0</span>, then the edge between vertexes <span class="tex-span"><i>i</i></span> and <span class="tex-span">(<i>i</i> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span> is directed from the <span class="tex-span"><i>i</i></span>-th vertex to the <span class="tex-span">(<i>i</i> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span>-th one, otherwise — to the opposite point.</p><p>It is guaranteed that the given graph is acyclic.</p></div><div class="output-specification"><p>Print a single integer — the size of the maximum antichain of graph <span class="tex-span"><i>G</i></span>.</p></div>

## Input

<p>The first line contains the sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">0</sub><i>s</i><sub class="lower-index">1</sub>... <i>s</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, consisting of numbers zero and one. The length of the line (number <span class="tex-span"><i>n</i></span>) corresponds to the number of vertexes and edges in graph <span class="tex-span"><i>G</i></span>. If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>i</i> ≥ 0)</span> equals <span class="tex-span">0</span>, then the edge between vertexes <span class="tex-span"><i>i</i></span> and <span class="tex-span">(<i>i</i> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span> is directed from the <span class="tex-span"><i>i</i></span>-th vertex to the <span class="tex-span">(<i>i</i> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span>-th one, otherwise — to the opposite point.</p><p>It is guaranteed that the given graph is acyclic.</p>

## Output

<p>Print a single integer — the size of the maximum antichain of graph <span class="tex-span"><i>G</i></span>.</p>





```input1
001

```




```input2
110010

```




```output1
1

```




```output2
3

```



## Note

<p>Consider the first test sample. The graph's <span class="tex-span"><i>G</i></span> edges are: <span class="tex-span">0 → 1</span>, <span class="tex-span">1 → 2</span>, <span class="tex-span">0 → 2</span>. We can choose the set of vertexes <span class="tex-span">[0]</span> as the maximum antichain. We cannot choose an antichain of larger size.</p>
