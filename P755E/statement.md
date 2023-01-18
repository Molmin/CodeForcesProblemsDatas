## Description

<div><p>PolandBall has an undirected simple graph consisting of <span class="tex-span"><i>n</i></span> vertices. Unfortunately, it has no edges. The graph is very sad because of that. PolandBall wanted to make it happier, adding some red edges. Then, he will add white edges in every remaining place. Therefore, the final graph will be a clique in two colors: white and red. </p><p>Colorfulness of the graph is a value <span class="tex-span"><i>min</i>(<i>d</i><sub class="lower-index"><i>r</i></sub>, <i>d</i><sub class="lower-index"><i>w</i></sub>)</span>, where <span class="tex-span"><i>d</i><sub class="lower-index"><i>r</i></sub></span> is the diameter of the red subgraph and <span class="tex-span"><i>d</i><sub class="lower-index"><i>w</i></sub></span> is the diameter of white subgraph. The diameter of a graph is a largest value <span class="tex-span"><i>d</i></span> such that shortest path between some pair of vertices in it is equal to <span class="tex-span"><i>d</i></span>. If the graph is not connected, we consider its diameter to be <span class="tex-font-style-tt">-1</span>.</p><p>PolandBall wants the final graph to be as neat as possible. He wants the final colorfulness to be equal to <span class="tex-span"><i>k</i></span>. Can you help him and find any graph which satisfies PolandBall's requests?</p></div><div class="input-specification"><p>The only one input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>), representing graph's size and sought colorfulness.</p></div><div class="output-specification"><p>If it's impossible to find a suitable graph, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, you can output any graph which fulfills PolandBall's requirements. First, output <span class="tex-span"><i>m</i></span>&nbsp;— the number of red edges in your graph. Then, you should output <span class="tex-span"><i>m</i></span> lines, each containing two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) which means that there is an undirected red edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Every red edge should be printed exactly once, you can print the edges and the vertices of every edge in arbitrary order.</p><p>Remember that PolandBall's graph should remain simple, so no loops or multiple edges are allowed.</p></div>

## Input

<p>The only one input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>), representing graph's size and sought colorfulness.</p>

## Output

<p>If it's impossible to find a suitable graph, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, you can output any graph which fulfills PolandBall's requirements. First, output <span class="tex-span"><i>m</i></span>&nbsp;— the number of red edges in your graph. Then, you should output <span class="tex-span"><i>m</i></span> lines, each containing two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) which means that there is an undirected red edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Every red edge should be printed exactly once, you can print the edges and the vertices of every edge in arbitrary order.</p><p>Remember that PolandBall's graph should remain simple, so no loops or multiple edges are allowed.</p>





```input1
4 1

```




```input2
5 2

```




```output1
-1

```




```output2
4
1 2
2 3
3 4
4 5

```



## Note

<p>In the first sample case, no graph can fulfill PolandBall's requirements.</p><p>In the second sample case, red graph is a path from <span class="tex-span">1</span> to <span class="tex-span">5</span>. Its diameter is <span class="tex-span">4</span>. However, white graph has diameter <span class="tex-span">2</span>, because it consists of edges <span class="tex-font-style-tt">1-3</span>, <span class="tex-font-style-tt">1-4</span>, <span class="tex-font-style-tt">1-5</span>, <span class="tex-font-style-tt">2-4</span>, <span class="tex-font-style-tt">2-5</span>, <span class="tex-font-style-tt">3-5</span>.</p>
