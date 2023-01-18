## Description

<div><p>You are given a bipartite graph <span class="tex-span"><i>G</i> = (<i>U</i>, <i>V</i>, <i>E</i>)</span>, <span class="tex-span"><i>U</i></span> is the set of vertices of the first part, <span class="tex-span"><i>V</i></span> is the set of vertices of the second part and <span class="tex-span"><i>E</i></span> is the set of edges. There might be multiple edges.</p><p>Let's call some subset of its edges <img align="middle" class="tex-formula" src="file://ZQGEBe6c.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-it"><span class="tex-span"><i>k</i></span>-covering</span> iff the graph <img align="middle" class="tex-formula" src="file://aOA5fx3p.png" style="max-width: 100.0%;max-height: 100.0%;"> has each of its vertices incident to at least <span class="tex-span"><i>k</i></span> edges. <span class="tex-font-style-it">Minimal <span class="tex-span"><i>k</i></span>-covering</span> is such a <span class="tex-span"><i>k</i></span>-covering that the size of the subset <img align="middle" class="tex-formula" src="file://zjKZeO05.png" style="max-width: 100.0%;max-height: 100.0%;"> is minimal possible.</p><p>Your task is to find minimal <span class="tex-span"><i>k</i></span>-covering for each <img align="middle" class="tex-formula" src="file://hl0SS7Ti.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>minDegree</i></span> is the minimal degree of any vertex in graph <span class="tex-span"><i>G</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2000</span>) — the number of vertices in the first part, the number of vertices in the second part and the number of edges, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i><sub class="lower-index">1</sub>, 1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i><sub class="lower-index">2</sub></span>) — the description of the <span class="tex-span"><i>i</i></span>-th edge, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the index of the vertex in the first part and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the index of the vertex in the second part.</p></div><div class="output-specification"><p>For each <img align="middle" class="tex-formula" src="file://8zQIg5DP.png" style="max-width: 100.0%;max-height: 100.0%;"> print the subset of edges (minimal <span class="tex-span"><i>k</i></span>-covering) in separate line.</p><p>The first integer <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>k</i></sub></span> of the <span class="tex-span"><i>k</i></span>-th line is the number of edges in minimal <span class="tex-span"><i>k</i></span>-covering of the graph. Then <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>k</i></sub></span> integers follow — original indices of the edges which belong to the minimal <span class="tex-span"><i>k</i></span>-covering, these indices should be pairwise distinct. Edges are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>m</i></span> in order they are given in the input.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2000</span>) — the number of vertices in the first part, the number of vertices in the second part and the number of edges, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i><sub class="lower-index">1</sub>, 1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i><sub class="lower-index">2</sub></span>) — the description of the <span class="tex-span"><i>i</i></span>-th edge, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the index of the vertex in the first part and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the index of the vertex in the second part.</p>

## Output

<p>For each <img align="middle" class="tex-formula" src="file://8zQIg5DP.png" style="max-width: 100.0%;max-height: 100.0%;"> print the subset of edges (minimal <span class="tex-span"><i>k</i></span>-covering) in separate line.</p><p>The first integer <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>k</i></sub></span> of the <span class="tex-span"><i>k</i></span>-th line is the number of edges in minimal <span class="tex-span"><i>k</i></span>-covering of the graph. Then <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>k</i></sub></span> integers follow — original indices of the edges which belong to the minimal <span class="tex-span"><i>k</i></span>-covering, these indices should be pairwise distinct. Edges are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>m</i></span> in order they are given in the input.</p>





```input1
3 3 7
1 2
2 3
1 3
3 2
3 3
2 1
2 1

```




```input2
1 1 5
1 1
1 1
1 1
1 1
1 1

```




```output1
0 
3 3 7 4 
6 1 3 6 7 4 5 

```




```output2
0 
1 5 
2 4 5 
3 3 4 5 
4 2 3 4 5 
5 1 2 3 4 5 

```


