## Description

<div><p><span class="tex-font-style-it">To your surprise, Jamie is the final boss! Ehehehe.</span></p><p>Jamie has given you a tree with <span class="tex-span"><i>n</i></span> vertices, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Initially, the root of the tree is the vertex with number <span class="tex-span">1</span>. Also, each vertex has a value on it.</p><p>Jamie also gives you three types of queries on the tree:</p><p><span class="tex-span">1 <i>v</i></span>&nbsp;— Change the tree's root to vertex with number <span class="tex-span"><i>v</i></span>.</p><p><span class="tex-span">2 <i>u</i> <i>v</i> <i>x</i></span>&nbsp;— For each vertex in the subtree of smallest size that contains <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, add <span class="tex-span"><i>x</i></span> to its value.</p><p><span class="tex-span">3 <i>v</i></span>&nbsp;— Find sum of values of vertices in the subtree of vertex with number <span class="tex-span"><i>v</i></span>.</p><p>A subtree of vertex <span class="tex-span"><i>v</i></span> is a set of vertices such that <span class="tex-span"><i>v</i></span> lies on shortest path from this vertex to root of the tree. Pay attention that subtree of a vertex can change after changing the tree's root.</p><p>Show your strength in programming to Jamie by performing the queries accurately!</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree and the number of queries to process respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— initial values of the vertices.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the tree.</p><p>The following <span class="tex-span"><i>q</i></span> lines describe the queries.</p><p>Each query has one of following formats depending on its type:</p><p><span class="tex-span">1 <i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) for queries of the first type.</p><p><span class="tex-span">2 <i>u</i> <i>v</i> <i>x</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>,  - 10<sup class="upper-index">8</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">8</sup></span>) for queries of the second type.</p><p><span class="tex-span">3 <i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) for queries of the third type.</p><p>All numbers in queries' descriptions are integers.</p><p>The queries must be carried out in the given order. It is guaranteed that the tree is valid.</p></div><div class="output-specification"><p>For each query of the third type, output the required answer. It is guaranteed that at least one query of the third type is given by Jamie.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree and the number of queries to process respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— initial values of the vertices.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the tree.</p><p>The following <span class="tex-span"><i>q</i></span> lines describe the queries.</p><p>Each query has one of following formats depending on its type:</p><p><span class="tex-span">1 <i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) for queries of the first type.</p><p><span class="tex-span">2 <i>u</i> <i>v</i> <i>x</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>,  - 10<sup class="upper-index">8</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">8</sup></span>) for queries of the second type.</p><p><span class="tex-span">3 <i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) for queries of the third type.</p><p>All numbers in queries' descriptions are integers.</p><p>The queries must be carried out in the given order. It is guaranteed that the tree is valid.</p>

## Output

<p>For each query of the third type, output the required answer. It is guaranteed that at least one query of the third type is given by Jamie.</p>





```input1
6 7
1 4 2 8 5 7
1 2
3 1
4 3
4 5
3 6
3 1
2 4 6 3
3 4
1 6
2 2 4 -5
1 4
3 3

```




```input2
4 6
4 3 5 6
1 2
2 3
3 4
3 1
1 3
2 2 4 3
1 1
2 2 4 -3
3 1

```




```output1
27
19
5

```




```output2
18
21

```



## Note

<p>The following picture shows how the tree varies after the queries in the first sample. </p><center> <img class="tex-graphics" src="file://C0mHmBxn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
