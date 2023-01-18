## Description

<div><p>Let's call an undirected graph of <span class="tex-span"><i>n</i></span> vertices <span class="tex-font-style-it"><span class="tex-span"><i>p</i></span>-interesting</span>, if the following conditions fulfill: </p><ul> <li> the graph contains exactly <span class="tex-span">2<i>n</i> + <i>p</i></span> edges; </li><li> the graph doesn't contain self-loops and multiple edges; </li><li> for any integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), any subgraph consisting of <span class="tex-span"><i>k</i></span> vertices contains at most <span class="tex-span">2<i>k</i> + <i>p</i></span> edges. </li></ul><p>A <span class="tex-font-style-it">subgraph</span> of a graph is some set of the graph vertices and some set of the graph edges. At that, the set of edges must meet the condition: both ends of each edge from the set must belong to the chosen set of vertices. </p><p>Your task is to find a <span class="tex-font-style-it"><span class="tex-span"><i>p</i></span>-interesting</span> graph consisting of <span class="tex-span"><i>n</i></span> vertices.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 5</span>) — the number of tests in the input. Next <span class="tex-span"><i>t</i></span> lines each contains two space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 24</span>; <span class="tex-span"><i>p</i> ≥ 0</span>; <img align="middle" class="tex-formula" src="file://2X6oMFAb.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of vertices in the graph and the interest value for the appropriate test. </p><p>It is guaranteed that the required graph exists.</p></div><div class="output-specification"><p>For each of the <span class="tex-span"><i>t</i></span> tests print <span class="tex-span">2<i>n</i> + <i>p</i></span> lines containing the description of the edges of a <span class="tex-font-style-it"><span class="tex-span"><i>p</i></span>-interesting</span> graph: the <span class="tex-span"><i>i</i></span>-th line must contain two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — two vertices, connected by an edge in the resulting graph. Consider the graph vertices numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>Print the answers to the tests in the order the tests occur in the input. If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 5</span>) — the number of tests in the input. Next <span class="tex-span"><i>t</i></span> lines each contains two space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 24</span>; <span class="tex-span"><i>p</i> ≥ 0</span>; <img align="middle" class="tex-formula" src="file://2X6oMFAb.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of vertices in the graph and the interest value for the appropriate test. </p><p>It is guaranteed that the required graph exists.</p>

## Output

<p>For each of the <span class="tex-span"><i>t</i></span> tests print <span class="tex-span">2<i>n</i> + <i>p</i></span> lines containing the description of the edges of a <span class="tex-font-style-it"><span class="tex-span"><i>p</i></span>-interesting</span> graph: the <span class="tex-span"><i>i</i></span>-th line must contain two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — two vertices, connected by an edge in the resulting graph. Consider the graph vertices numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>Print the answers to the tests in the order the tests occur in the input. If there are multiple solutions, you can print any of them.</p>





```input1
1
6 0

```




```output1
1 2
1 3
1 4
1 5
1 6
2 3
2 4
2 5
2 6
3 4
3 5
3 6

```


