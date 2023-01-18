## Description

<div><p>Hexadecimal likes drawing. She has drawn many graphs already, both directed and not. Recently she has started to work on a still-life «interesting graph and apples». An undirected graph is called interesting, if each of its vertices belongs to one cycle only — a funny ring — and does not belong to any other cycles. A funny ring is a cycle that goes through all the vertices just once. Moreover, loops are funny rings too.</p><p>She has already drawn the apples and some of the graph edges. But now it is not clear, how to connect the rest of the vertices to get an interesting graph as a result. The answer should contain the minimal amount of added edges. And furthermore, the answer should be the lexicographically smallest one. The set of edges <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>), (<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>), ..., (<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub></span>, is lexicographically smaller than the set <span class="tex-span">(<i>u</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">1</sub>), (<i>u</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">2</sub>), ..., (<i>u</i><sub class="lower-index"><i>n</i></sub>, <i>v</i><sub class="lower-index"><i>n</i></sub>)</span>, where <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, provided that the sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub></span> is lexicographically smaller than the sequence <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub>, <i>v</i><sub class="lower-index"><i>n</i></sub></span>. If you do not cope, Hexadecimal will eat you. ...eat you alive.</p></div><div class="input-specification"><p>The first line of the input data contains a pair of integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2500</span>) — the amount of vertices and edges respectively. The following lines contain pairs of numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the vertices that are already connected by edges. The initial graph may contain multiple edges and loops.</p></div><div class="output-specification"><p>In the first line output «<span class="tex-font-style-tt">YES</span>» or «<span class="tex-font-style-tt">NO</span>»: if it is possible or not to construct an interesting graph. If the answer is «<span class="tex-font-style-tt">YES</span>», in the second line output <span class="tex-span"><i>k</i></span> — the amount of edges that should be added to the initial graph. Finally, output <span class="tex-span"><i>k</i></span> lines: pairs of vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>, between which edges should be drawn. The result may contain multiple edges and loops. <span class="tex-span"><i>k</i></span> can be equal to zero.</p></div>

## Input

<p>The first line of the input data contains a pair of integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2500</span>) — the amount of vertices and edges respectively. The following lines contain pairs of numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the vertices that are already connected by edges. The initial graph may contain multiple edges and loops.</p>

## Output

<p>In the first line output «<span class="tex-font-style-tt">YES</span>» or «<span class="tex-font-style-tt">NO</span>»: if it is possible or not to construct an interesting graph. If the answer is «<span class="tex-font-style-tt">YES</span>», in the second line output <span class="tex-span"><i>k</i></span> — the amount of edges that should be added to the initial graph. Finally, output <span class="tex-span"><i>k</i></span> lines: pairs of vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>, between which edges should be drawn. The result may contain multiple edges and loops. <span class="tex-span"><i>k</i></span> can be equal to zero.</p>





```input1
3 2
1 2
2 3

```




```output1
YES
1
1 3

```


