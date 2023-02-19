## Description

<div><p>Vanya wants to minimize a tree. He can perform the following operation multiple times: choose a vertex <span class="tex-span"><i>v</i></span>, and two disjoint (except for <span class="tex-span"><i>v</i></span>) paths of equal length <span class="tex-span"><i>a</i><sub class="lower-index">0</sub> = <i>v</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, and <span class="tex-span"><i>b</i><sub class="lower-index">0</sub> = <i>v</i></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>. Additionally, vertices <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> must not have any neighbours in the tree other than adjacent vertices of corresponding paths. After that, one of the paths may be merged into the other, that is, the vertices <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> can be effectively erased:</p><center> <img class="tex-graphics" src="file://3oEPnrxB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help Vanya determine if it possible to make the tree into a path via a sequence of described operations, and if the answer is positive, also determine the shortest length of such path.</p></div><div class="input-specification"><p>The first line of input contains the number of vertices <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe edges of the tree. Each of these lines contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>)&nbsp;— indices of endpoints of the corresponding edge. It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>If it is impossible to obtain a path, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum number of edges in a possible path.</p></div>

## Input

<p>The first line of input contains the number of vertices <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe edges of the tree. Each of these lines contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>)&nbsp;— indices of endpoints of the corresponding edge. It is guaranteed that the given graph is a tree.</p>

## Output

<p>If it is impossible to obtain a path, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum number of edges in a possible path.</p>





```input1
6
1 2
2 3
2 4
4 5
1 6

```




```input2
7
1 2
1 3
3 4
1 5
5 6
6 7

```




```output1
3

```




```output2
-1

```



## Note

<p>In the first sample case, a path of three edges is obtained after merging paths <span class="tex-span">2 - 1 - 6</span> and <span class="tex-span">2 - 4 - 5</span>.</p><p>It is impossible to perform any operation in the second sample case. For example, it is impossible to merge paths <span class="tex-span">1 - 3 - 4</span> and <span class="tex-span">1 - 5 - 6</span>, since vertex 6 additionally has a neighbour 7 that is not present in the corresponding path.</p>
