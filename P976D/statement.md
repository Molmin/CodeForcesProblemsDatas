## Description

<div><p>You are given a sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>d</i><sub class="lower-index">1</sub> &lt; <i>d</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>d</i><sub class="lower-index"><i>n</i></sub></span>). Your task is to construct an undirected graph such that:</p><ul> <li> there are exactly <span class="tex-span"><i>d</i><sub class="lower-index"><i>n</i></sub> + 1</span> vertices; </li><li> there are no self-loops; </li><li> there are no multiple edges; </li><li> there are no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> edges; </li><li> its <span class="tex-font-style-it">degree set</span> is equal to <span class="tex-span"><i>d</i></span>. </li></ul><p>Vertices should be numbered <span class="tex-span">1</span> through <span class="tex-span">(<i>d</i><sub class="lower-index"><i>n</i></sub> + 1)</span>.</p><p><span class="tex-font-style-it">Degree sequence</span> is an array <span class="tex-span"><i>a</i></span> with length equal to the number of vertices in a graph such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of vertices adjacent to <span class="tex-span"><i>i</i></span>-th vertex.</p><p><span class="tex-font-style-it">Degree set</span> is a sorted in increasing order sequence of all distinct values from the <span class="tex-font-style-it">degree sequence</span>.</p><p>It is guaranteed that there exists such a graph that all the conditions hold, and it contains no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> edges.</p><p>Print the resulting graph.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the size of the degree set.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span"><i>d</i><sub class="lower-index">1</sub> &lt; <i>d</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>d</i><sub class="lower-index"><i>n</i></sub></span>) — the degree set.</p></div><div class="output-specification"><p>In the first line print one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of edges in the resulting graph. It is guaranteed that there exists such a graph that all the conditions hold and it contains no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> edges.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines should contain two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>n</i></sub> + 1</span>) — the description of the <span class="tex-span"><i>i</i></span>-th edge.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the size of the degree set.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span"><i>d</i><sub class="lower-index">1</sub> &lt; <i>d</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>d</i><sub class="lower-index"><i>n</i></sub></span>) — the degree set.</p>

## Output

<p>In the first line print one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of edges in the resulting graph. It is guaranteed that there exists such a graph that all the conditions hold and it contains no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> edges.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines should contain two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>n</i></sub> + 1</span>) — the description of the <span class="tex-span"><i>i</i></span>-th edge.</p>





```input1
3
2 3 4

```




```input2
3
1 2 3

```




```output1
8
3 1
4 2
4 5
2 5
5 1
3 2
2 1
5 3

```




```output2
4
1 2
1 3
1 4
2 3

```


