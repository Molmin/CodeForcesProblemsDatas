## Description

<div><p>In this problem you have to build tournament graph, consisting of <span class="tex-span"><i>n</i></span> vertices, such, that for any oriented pair of vertices <span class="tex-span">(<i>v</i>, <i>u</i>)</span> <span class="tex-span">(<i>v</i> ≠ <i>u</i>)</span> there exists a path from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span> consisting of no more then two edges.</p><p>A directed graph without self-loops is a <span class="tex-font-style-it">tournament</span>, if there is exactly one edge between any two distinct vertices (in one out of two possible directions).</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 1000)</span>, the number of the graph's vertices.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if there is no graph, satisfying the described conditions.</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> integers in each. The numbers should be separated with spaces. That is adjacency matrix <span class="tex-span"><i>a</i></span> of the found tournament. Consider the graph vertices to be numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Then <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>u</i></sub> = 0</span>, if there is no edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>u</i></sub> = 1</span> if there is one. </p><p>As the output graph has to be a tournament, following equalities must be satisfied: </p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>u</i></sub> + <i>a</i><sub class="lower-index"><i>u</i>, <i>v</i></sub> = 1</span> for each <span class="tex-span"><i>v</i>, <i>u</i></span> <span class="tex-span">(1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>;&nbsp;<i>v</i> ≠ <i>u</i>)</span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>v</i></sub> = 0</span> for each <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>v</i> ≤ <i>n</i>)</span>. </li></ul></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 1000)</span>, the number of the graph's vertices.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if there is no graph, satisfying the described conditions.</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> integers in each. The numbers should be separated with spaces. That is adjacency matrix <span class="tex-span"><i>a</i></span> of the found tournament. Consider the graph vertices to be numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Then <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>u</i></sub> = 0</span>, if there is no edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>u</i></sub> = 1</span> if there is one. </p><p>As the output graph has to be a tournament, following equalities must be satisfied: </p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>u</i></sub> + <i>a</i><sub class="lower-index"><i>u</i>, <i>v</i></sub> = 1</span> for each <span class="tex-span"><i>v</i>, <i>u</i></span> <span class="tex-span">(1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>;&nbsp;<i>v</i> ≠ <i>u</i>)</span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i>, <i>v</i></sub> = 0</span> for each <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>v</i> ≤ <i>n</i>)</span>. </li></ul>





```input1
3

```




```input2
4

```




```output1
0 1 0
0 0 1
1 0 0

```




```output2
-1

```


