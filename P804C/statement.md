## Description

<div><p>Isart and Modsart were trying to solve an interesting problem when suddenly Kasra arrived. Breathless, he asked: "Can you solve a problem I'm stuck at all day?"</p><p>We have a tree <span class="tex-span"><i>T</i></span> with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> types of ice cream numerated from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Each vertex <span class="tex-span"><i>i</i></span> has a set of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> types of ice cream. Vertices which have the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) type of ice cream form a connected subgraph. We build a new graph <span class="tex-span"><i>G</i></span> with <span class="tex-span"><i>m</i></span> vertices. We put an edge between the <span class="tex-span"><i>v</i></span>-th and the <span class="tex-span"><i>u</i></span>-th (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>m</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>) vertices in <span class="tex-span"><i>G</i></span> if and only if there exists a vertex in <span class="tex-span"><i>T</i></span> that has both the <span class="tex-span"><i>v</i></span>-th and the <span class="tex-span"><i>u</i></span>-th types of ice cream in its set. The problem is to paint the vertices of <span class="tex-span"><i>G</i></span> with minimum possible number of colors in a way that no adjacent vertices have the same color.</p><p>Please note that we consider that empty set of vertices form a connected subgraph in this problem.</p><p>As usual, Modsart don't like to abandon the previous problem, so Isart wants you to solve the new problem.</p></div><div class="input-specification"><p>The first line contains two integer <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in <span class="tex-span"><i>T</i></span> and the number of ice cream types.</p><p><span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of these lines contain single integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>) and then <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> distinct integers, each between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>&nbsp;— the types of ice cream in the <span class="tex-span"><i>i</i></span>-th vertex. The sum of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p><p><span class="tex-span"><i>n</i> - 1</span> lines follow. Each of these lines describes an edge of the tree with two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>)&nbsp;— the indexes of connected by this edge vertices.</p></div><div class="output-specification"><p>Print single integer <span class="tex-span"><i>c</i></span> in the first line&nbsp;— the minimum number of colors to paint the vertices in graph <span class="tex-span"><i>G</i></span>.</p><p>In the second line print <span class="tex-span"><i>m</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of which should be the color of the <span class="tex-span"><i>i</i></span>-th vertex. The colors should be between <span class="tex-span">1</span> and <span class="tex-span"><i>c</i></span>. If there are some answers, print any of them.</p></div>

## Input

<p>The first line contains two integer <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in <span class="tex-span"><i>T</i></span> and the number of ice cream types.</p><p><span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of these lines contain single integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>) and then <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> distinct integers, each between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>&nbsp;— the types of ice cream in the <span class="tex-span"><i>i</i></span>-th vertex. The sum of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p><p><span class="tex-span"><i>n</i> - 1</span> lines follow. Each of these lines describes an edge of the tree with two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>)&nbsp;— the indexes of connected by this edge vertices.</p>

## Output

<p>Print single integer <span class="tex-span"><i>c</i></span> in the first line&nbsp;— the minimum number of colors to paint the vertices in graph <span class="tex-span"><i>G</i></span>.</p><p>In the second line print <span class="tex-span"><i>m</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of which should be the color of the <span class="tex-span"><i>i</i></span>-th vertex. The colors should be between <span class="tex-span">1</span> and <span class="tex-span"><i>c</i></span>. If there are some answers, print any of them.</p>





```input1
3 3
1 1
2 2 3
1 2
1 2
2 3

```




```input2
4 5
0
1 1
1 3
3 2 4 5
2 1
3 2
4 3

```




```output1
2
1 1 2
```




```output2
3
1 1 1 2 3
```



## Note

<p>In the first example the first type of ice cream is present in the first vertex only, so we can color it in any color. The second and the third ice cream are both presented in the second vertex, so we should paint them in different colors.</p><p>In the second example the colors of the second, the fourth and the fifth ice cream should obviously be distinct.</p>
