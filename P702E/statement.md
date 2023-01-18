## Description

<div><p>You are given a <span class="tex-font-style-it">functional graph</span>. It is a directed graph, in which from each vertex goes exactly one arc. The vertices are numerated from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>.</p><p>Graph is given as the array <span class="tex-span"><i>f</i><sub class="lower-index">0</sub>, <i>f</i><sub class="lower-index">1</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> — the number of vertex to which goes the only arc from the vertex <span class="tex-span"><i>i</i></span>. Besides you are given array with weights of the arcs <span class="tex-span"><i>w</i><sub class="lower-index">0</sub>, <i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> — the arc weight from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>.</p><center> <img class="tex-graphics" src="file://6Fa1B51P.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The graph from the first sample test.</span> </center><p>Also you are given the integer <span class="tex-span"><i>k</i></span> (the length of the path) and you need to find for each vertex two numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, where:</p><ul> <li> <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> — the sum of the weights of all arcs of the path with length equals to <span class="tex-span"><i>k</i></span> which starts from the vertex <span class="tex-span"><i>i</i></span>; </li><li> <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> — the minimal weight from all arcs on the path with length <span class="tex-span"><i>k</i></span> which starts from the vertex <span class="tex-span"><i>i</i></span>. </li></ul><p>The length of the path is the number of arcs on this path.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">10</sup></span>). The second line contains the sequence <span class="tex-span"><i>f</i><sub class="lower-index">0</sub>, <i>f</i><sub class="lower-index">1</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>) and the third — the sequence <span class="tex-span"><i>w</i><sub class="lower-index">0</sub>, <i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, the pair of integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> in each line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">10</sup></span>). The second line contains the sequence <span class="tex-span"><i>f</i><sub class="lower-index">0</sub>, <i>f</i><sub class="lower-index">1</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>) and the third — the sequence <span class="tex-span"><i>w</i><sub class="lower-index">0</sub>, <i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, the pair of integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> in each line.</p>





```input1
7 3
1 2 3 4 3 2 6
6 3 1 4 2 2 3

```




```input2
4 4
0 1 2 3
0 1 2 3

```




```input3
5 3
1 2 3 4 0
4 1 2 14 3

```




```output1
10 1
8 1
7 1
10 2
8 2
7 1
9 3

```




```output2
0 0
4 1
8 2
12 3

```




```output3
7 1
17 1
19 2
21 3
8 1

```


