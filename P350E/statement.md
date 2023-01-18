## Description

<div><p>Valera conducts experiments with algorithms that search for shortest paths. He has recently studied the Floyd's algorithm, so it's time to work with it.</p><p>Valera's already written the code that counts the shortest distance between any pair of vertexes in a <span class="tex-font-style-bf">non-directed connected graph</span> from <span class="tex-span"><i>n</i></span> vertexes and <span class="tex-span"><i>m</i></span> edges, containing no loops and multiple edges. Besides, Valera's decided to mark part of the vertexes. He's marked exactly <span class="tex-span"><i>k</i></span> vertexes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Valera's code is given below.</p><pre class="verbatim"><br>ans[i][j] // the shortest distance for a pair of vertexes <span class="tex-span"><i>i</i>, <i>j</i></span><br>a[i]  // vertexes, marked by Valera<br><br>for(i = 1; i &lt;= n; i++) {<br>    for(j = 1; j &lt;= n; j++) {<br>        if (i == j)<br>            ans[i][j] = 0;<br>        else<br>            ans[i][j] = INF;  //INF is a very large number <br>    }<br>}    <br><br>for(i = 1; i &lt;= m; i++) {<br>    read a pair of vertexes u, v that have a non-directed edge between them;<br>    ans[u][v] = 1;<br>    ans[v][u] = 1;<br>}<br><br>for (i = 1; i &lt;= k; i++) {<br>    v = a[i];<br>    for(j = 1; j &lt;= n; j++)<br>        for(r = 1; r &lt;= n; r++)<br>            ans[j][r] = min(ans[j][r], ans[j][v] + ans[v][r]);<br>}<br></pre><p>Valera has seen that his code is wrong. Help the boy. Given the set of marked vertexes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, find such <span class="tex-font-style-bf">non-directed connected graph</span>, consisting of <span class="tex-span"><i>n</i></span> vertexes and <span class="tex-span"><i>m</i></span> edges, for which Valera's code counts the wrong shortest distance for at least one pair of vertexes <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. Valera is really keen to get a graph without any loops and multiple edges. If no such graph exists, print -1.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i></span> , <img align="middle" class="tex-formula" src="file://Y0QZT9Yc.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of vertexes, the number of edges and the number of marked vertexes. </p><p>The second line of the input contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the numbers of the marked vertexes. It is guaranteed that all numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>If the graph doesn't exist, print -1 on a single line. Otherwise, print <span class="tex-span"><i>m</i></span> lines, each containing two integers <span class="tex-span"><i>u</i>, <i>v</i></span> — the description of the edges of the graph Valera's been looking for.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i></span> , <img align="middle" class="tex-formula" src="file://Y0QZT9Yc.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of vertexes, the number of edges and the number of marked vertexes. </p><p>The second line of the input contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the numbers of the marked vertexes. It is guaranteed that all numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>If the graph doesn't exist, print -1 on a single line. Otherwise, print <span class="tex-span"><i>m</i></span> lines, each containing two integers <span class="tex-span"><i>u</i>, <i>v</i></span> — the description of the edges of the graph Valera's been looking for.</p>





```input1
3 2 2
1 2

```




```input2
3 3 2
1 2

```




```output1
1 3
2 3

```




```output2
-1

```


