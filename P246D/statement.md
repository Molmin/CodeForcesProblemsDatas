## Description

<div><p>You've got an undirected graph, consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. We will consider the graph's vertices numbered with integers from 1 to <span class="tex-span"><i>n</i></span>. Each vertex of the graph has a color. The color of the <span class="tex-span"><i>i</i></span>-th vertex is an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Let's consider all vertices of the graph, that are painted some color <span class="tex-span"><i>k</i></span>. Let's denote a set of such as <span class="tex-span"><i>V</i>(<i>k</i>)</span>. Let's denote the value of the <span class="tex-font-style-it">neighbouring color diversity</span> for color <span class="tex-span"><i>k</i></span> as the cardinality of the set <span class="tex-span"><i>Q</i>(<i>k</i>) = {<i>c</i><sub class="lower-index"><i>u</i></sub>&nbsp;: &nbsp;<i>c</i><sub class="lower-index"><i>u</i></sub> ≠ <i>k</i></span> and there is vertex <span class="tex-span"><i>v</i></span> belonging to set <span class="tex-span"><i>V</i>(<i>k</i>)</span> such that nodes <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> are connected by an edge of the graph<span class="tex-span">}</span>.</p><p>Your task is to find such color <span class="tex-span"><i>k</i></span>, which makes the cardinality of set <span class="tex-span"><i>Q</i>(<i>k</i>)</span> maximum. In other words, you want to find the color that has the most diverse neighbours. Please note, that you want to find such color <span class="tex-span"><i>k</i></span>, that the graph has at least one vertex with such color.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices end edges of the graph, correspondingly. The second line contains a sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the colors of the graph vertices. The numbers on the line are separated by spaces.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the edges: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers of the vertices, connected by the <span class="tex-span"><i>i</i></span>-th edge. </p><p>It is guaranteed that the given graph has no self-loops or multiple edges.</p></div><div class="output-specification"><p>Print the number of the color which has the set of neighbours with the maximum cardinality. It there are multiple optimal colors, print the color with the minimum number. Please note, that you want to find such color, that the graph has at least one vertex with such color.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices end edges of the graph, correspondingly. The second line contains a sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the colors of the graph vertices. The numbers on the line are separated by spaces.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the edges: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers of the vertices, connected by the <span class="tex-span"><i>i</i></span>-th edge. </p><p>It is guaranteed that the given graph has no self-loops or multiple edges.</p>

## Output

<p>Print the number of the color which has the set of neighbours with the maximum cardinality. It there are multiple optimal colors, print the color with the minimum number. Please note, that you want to find such color, that the graph has at least one vertex with such color.</p>





```input1
6 6
1 1 2 3 5 8
1 2
3 2
1 4
4 3
4 5
4 6

```




```input2
5 6
4 2 5 2 4
1 2
2 3
3 1
5 3
5 4
3 4

```




```output1
3

```




```output2
2

```


