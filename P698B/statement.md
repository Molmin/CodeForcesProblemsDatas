## Description

<div><p>A tree is an undirected connected graph without cycles.</p><p>Let's consider a rooted undirected tree with <span class="tex-span"><i>n</i></span> vertices, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. There are many ways to represent such a tree. One way is to create an array with <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes a parent of vertex <span class="tex-span"><i>i</i></span> (here, for convenience a root is considered its own parent).</p><center> <img class="tex-graphics" src="file://GW8TBWK2.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">For this rooted tree the array <span class="tex-span"><i>p</i></span> is <span class="tex-span">[2, 3, 3, 2]</span>.</span> </center><p>Given a sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, one is able to restore a tree:</p><ol> <li> There must be exactly one index <span class="tex-span"><i>r</i></span> that <span class="tex-span"><i>p</i><sub class="lower-index"><i>r</i></sub> = <i>r</i></span>. A vertex <span class="tex-span"><i>r</i></span> is a root of the tree. </li><li> For all other <span class="tex-span"><i>n</i> - 1</span> vertices <span class="tex-span"><i>i</i></span>, there is an edge between vertex <span class="tex-span"><i>i</i></span> and vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. </li></ol><p>A sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> is called valid if the described procedure generates some (any) rooted tree. For example, for <span class="tex-span"><i>n</i> = 3</span> sequences <span class="tex-font-style-tt">(1,2,2)</span>, <span class="tex-font-style-tt">(2,3,1)</span> and <span class="tex-font-style-tt">(2,1,3)</span> <span class="tex-font-style-bf">are not</span> valid.</p><p>You are given a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, not necessarily valid. Your task is to change the minimum number of elements, in order to get a valid sequence. Print the minimum number of changes and an example of a valid sequence after that number of changes. If there are many valid sequences achievable in the minimum number of changes, print any of them.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>In the first line print the minimum number of elements to change, in order to get a valid sequence.</p><p>In the second line, print any valid sequence possible to get from <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> in the minimum number of changes. If there are many such sequences, any of them will be accepted.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>In the first line print the minimum number of elements to change, in order to get a valid sequence.</p><p>In the second line, print any valid sequence possible to get from <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> in the minimum number of changes. If there are many such sequences, any of them will be accepted.</p>





```input1
4
2 3 3 4

```




```input2
5
3 2 2 5 3

```




```input3
8
2 3 5 4 1 6 6 7

```




```output1
1
2 3 4 4 

```




```output2
0
3 2 2 5 3 

```




```output3
2
2 3 7 8 1 6 6 7

```



## Note

<p>In the first sample, it's enough to change one element. In the provided output, a sequence represents a tree rooted in a vertex <span class="tex-span">4</span> (because <span class="tex-span"><i>p</i><sub class="lower-index">4</sub> = 4</span>), which you can see on the left drawing below. One of other correct solutions would be a sequence <span class="tex-font-style-tt">2 3 3 2</span>, representing a tree rooted in vertex <span class="tex-span">3</span> (right drawing below). On both drawings, roots are painted red.</p><center> <img class="tex-graphics" src="file://KBJxUfup.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, the given sequence is already valid.</p>
