## Description

<div><p>Ivan is developing his own computer game. Now he tries to create some levels for his game. But firstly for each level he needs to draw a graph representing the structure of the level.</p><p>Ivan decided that there should be exactly <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> vertices in the graph representing level <span class="tex-span"><i>i</i></span>, and the edges have to be bidirectional. When constructing the graph, Ivan is interested in special edges called <span class="tex-font-style-it">bridges</span>. An edge between two vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is called a <span class="tex-font-style-it">bridge</span> if this edge belongs to every path between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (and these vertices will belong to different connected components if we delete this edge). For each level Ivan wants to construct a graph where at least half of the edges are <span class="tex-font-style-it">bridges</span>. He also wants to maximize the number of edges in each constructed graph.</p><p>So the task Ivan gave you is: given <span class="tex-span"><i>q</i></span> numbers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub>, ..., <i>n</i><sub class="lower-index"><i>q</i></sub></span>, for each <span class="tex-span"><i>i</i></span> tell the maximum number of edges in a graph with <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> vertices, if at least half of the edges are <span class="tex-font-style-it">bridges</span>. <span class="tex-font-style-bf">Note that the graphs cannot contain multiple edges or self-loops</span>.</p></div><div class="input-specification"><p>The first line of input file contains a positive integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>) — the number of graphs Ivan needs to construct.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line contains one positive integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of vertices in <span class="tex-span"><i>i</i></span>-th graph.</p><p><span class="tex-font-style-it">Note that in hacks you have to use <span class="tex-span"><i>q</i> = 1</span>.</span></p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> numbers, <span class="tex-span"><i>i</i></span>-th of them must be equal to the maximum number of edges in <span class="tex-span"><i>i</i></span>-th graph.</p></div>

## Input

<p>The first line of input file contains a positive integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>) — the number of graphs Ivan needs to construct.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line contains one positive integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of vertices in <span class="tex-span"><i>i</i></span>-th graph.</p><p><span class="tex-font-style-it">Note that in hacks you have to use <span class="tex-span"><i>q</i> = 1</span>.</span></p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> numbers, <span class="tex-span"><i>i</i></span>-th of them must be equal to the maximum number of edges in <span class="tex-span"><i>i</i></span>-th graph.</p>





```input1
3
3
4
6

```




```output1
2
3
6

```



## Note

<p>In the first example it is possible to construct these graphs:</p><ol> <li> <span class="tex-span">1 - 2</span>, <span class="tex-span">1 - 3</span>; </li><li> <span class="tex-span">1 - 2</span>, <span class="tex-span">1 - 3</span>, <span class="tex-span">2 - 4</span>; </li><li> <span class="tex-span">1 - 2</span>, <span class="tex-span">1 - 3</span>, <span class="tex-span">2 - 3</span>, <span class="tex-span">1 - 4</span>, <span class="tex-span">2 - 5</span>, <span class="tex-span">3 - 6</span>. </li></ol>
