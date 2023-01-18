## Description

<div><p>Student Vladislav came to his programming exam completely unprepared as usual. He got a question about some strange algorithm on a graph&nbsp;— something that will definitely never be useful in real life. He asked a girl sitting next to him to lend him some cheat papers for this questions and found there the following definition:</p><p><span class="tex-font-style-it">The minimum spanning tree</span> <span class="tex-span"><i>T</i></span> of graph <span class="tex-span"><i>G</i></span> is such a tree that it contains all the vertices of the original graph <span class="tex-span"><i>G</i></span>, and the sum of the weights of its edges is the minimum possible among all such trees.</p><p>Vladislav drew a graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges containing no loops and multiple edges. He found one of its minimum spanning trees and then wrote for each edge its weight and whether it is included in the found tree or not. Unfortunately, the piece of paper where the graph was painted is gone and the teacher is getting very angry and demands to see the original graph. Help Vladislav come up with a graph so that the information about the minimum spanning tree remains correct.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://d0CVKanT.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of vertices and the number of edges in the graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines describes an edge of the graph and consists of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>b</i><sub class="lower-index"><i>j</i></sub> = {0, 1}</span>). The first of these numbers is the weight of the edge and the second number is equal to <span class="tex-span">1</span> if this edge was included in the minimum spanning tree found by Vladislav, or <span class="tex-span">0</span> if it was not.</p><p>It is guaranteed that exactly <span class="tex-span"><i>n</i> - 1</span> number <span class="tex-span">{<i>b</i><sub class="lower-index"><i>j</i></sub>}</span> are equal to one and exactly <span class="tex-span"><i>m</i> - <i>n</i> + 1</span> of them are equal to zero.</p></div><div class="output-specification"><p>If Vladislav has made a mistake and such graph doesn't exist, print <span class="tex-span"> - 1</span>.</p><p>Otherwise print <span class="tex-span"><i>m</i></span> lines. On the <span class="tex-span"><i>j</i></span>-th line print a pair of vertices <span class="tex-span">(<i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub>)</span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span>), that should be connected by the <span class="tex-span"><i>j</i></span>-th edge. The edges are numbered in the same order as in the input. The graph, determined by these edges, must be connected, contain no loops or multiple edges and its edges with <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> = 1</span> must define the minimum spanning tree. In case there are multiple possible solutions, print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://d0CVKanT.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of vertices and the number of edges in the graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines describes an edge of the graph and consists of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>b</i><sub class="lower-index"><i>j</i></sub> = {0, 1}</span>). The first of these numbers is the weight of the edge and the second number is equal to <span class="tex-span">1</span> if this edge was included in the minimum spanning tree found by Vladislav, or <span class="tex-span">0</span> if it was not.</p><p>It is guaranteed that exactly <span class="tex-span"><i>n</i> - 1</span> number <span class="tex-span">{<i>b</i><sub class="lower-index"><i>j</i></sub>}</span> are equal to one and exactly <span class="tex-span"><i>m</i> - <i>n</i> + 1</span> of them are equal to zero.</p>

## Output

<p>If Vladislav has made a mistake and such graph doesn't exist, print <span class="tex-span"> - 1</span>.</p><p>Otherwise print <span class="tex-span"><i>m</i></span> lines. On the <span class="tex-span"><i>j</i></span>-th line print a pair of vertices <span class="tex-span">(<i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub>)</span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span>), that should be connected by the <span class="tex-span"><i>j</i></span>-th edge. The edges are numbered in the same order as in the input. The graph, determined by these edges, must be connected, contain no loops or multiple edges and its edges with <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> = 1</span> must define the minimum spanning tree. In case there are multiple possible solutions, print any of them.</p>





```input1
4 5
2 1
3 1
4 0
1 1
5 0

```




```input2
3 3
1 0
2 1
3 1

```




```output1
2 4
1 4
3 4
3 1
3 2

```




```output2
-1

```


