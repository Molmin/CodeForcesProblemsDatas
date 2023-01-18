## Description

<div><p>Leha plays a computer game, where is on each level is given a connected graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. Graph can contain multiple edges, but can not contain self loops. Each vertex has an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, which can be equal to <span class="tex-span">0</span>, <span class="tex-span">1</span> or <span class="tex-span"> - 1</span>. To pass the level, he needs to find a «good» subset of edges of the graph or say, that it doesn't exist. Subset is called «good», if by by leaving only edges from this subset in the original graph, we obtain the following: for every vertex i, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> =  - 1 or it's degree modulo 2 is equal to <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Leha wants to pass the game as soon as possible and ask you to help him. In case of multiple correct answers, print any of them.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — number of vertices and edges.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — numbers on the vertices.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) — edges. It's guaranteed, that graph in the input is connected.</p></div><div class="output-specification"><p>Print <span class="tex-span"> - 1</span> in a single line, if solution doesn't exist. Otherwise in the first line <span class="tex-span"><i>k</i></span> — number of edges in a subset. In the next <span class="tex-span"><i>k</i></span> lines indexes of edges. Edges are numerated in order as they are given in the input, starting from <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — number of vertices and edges.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — numbers on the vertices.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) — edges. It's guaranteed, that graph in the input is connected.</p>

## Output

<p>Print <span class="tex-span"> - 1</span> in a single line, if solution doesn't exist. Otherwise in the first line <span class="tex-span"><i>k</i></span> — number of edges in a subset. In the next <span class="tex-span"><i>k</i></span> lines indexes of edges. Edges are numerated in order as they are given in the input, starting from <span class="tex-span">1</span>.</p>





```input1
1 0
1

```




```input2
4 5
0 0 0 -1
1 2
2 3
3 4
1 4
2 4

```




```input3
2 1
1 1
1 2

```




```input4
3 3
0 -1 1
1 2
2 3
1 3

```




```output1
-1

```




```output2
0

```




```output3
1
1

```




```output4
1
2

```



## Note

<p>In the first sample we have single vertex without edges. It's degree is 0 and we can not get 1.</p>
