## Description

<div><p>When Adam gets a rooted tree (connected non-directed graph without cycles), he immediately starts coloring it. More formally, he assigns a color to each edge of the tree so that it meets the following two conditions: </p><ul> <li> There is no vertex that has more than two incident edges painted the same color. </li><li> For any two vertexes that have incident edges painted the same color (say, <span class="tex-span"><i>c</i></span>), the path between them consists of the edges of the color <span class="tex-span"><i>c</i></span>. </li></ul><p>Not all tree paintings are equally good for Adam. Let's consider the path from some vertex to the root. Let's call the number of distinct colors on this path the cost of the vertex. The cost of the tree's coloring will be the maximum cost among all the vertexes. Help Adam determine the minimum possible cost of painting the tree. </p><p>Initially, Adam's tree consists of a single vertex that has number one and is the root. In one move Adam adds a new vertex to the already existing one, the new vertex gets the number equal to the minimum positive available integer. After each operation you need to calculate the minimum cost of coloring the resulting tree.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of times a new vertex is added. The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>) — the numbers of the vertexes to which we add another vertex. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers — the minimum costs of the tree painting after each addition. </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of times a new vertex is added. The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>) — the numbers of the vertexes to which we add another vertex. </p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers — the minimum costs of the tree painting after each addition. </p>





```input1
11
1 1 1 3 4 4 7 3 7 6 6

```




```output1
1 1 1 1 1 2 2 2 2 2 3
```



## Note

<p>The figure below shows one of the possible variants to paint a tree from the sample at the last moment. The cost of the vertexes with numbers 11 and 12 equals 3.</p><p><img class="tex-graphics" src="file://sspG1o33.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
