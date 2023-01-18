## Description

<div><p>Alyona decided to go on a diet and went to the forest to get some apples. There she unexpectedly found a magic rooted tree with root in the vertex <span class="tex-span">1</span>, every vertex and every edge of which has a number written on.</p><p>The girl noticed that some of the tree's vertices are <span class="tex-font-style-it">sad</span>, so she decided to play with them. Let's call vertex <span class="tex-span"><i>v</i></span> <span class="tex-font-style-it">sad</span> if there is a vertex <span class="tex-span"><i>u</i></span> in subtree of vertex <span class="tex-span"><i>v</i></span> such that <span class="tex-span"><i>dist</i>(<i>v</i>, <i>u</i>) &gt; <i>a</i><sub class="lower-index"><i>u</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>u</i></sub></span> is the number written on vertex <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>dist</i>(<i>v</i>, <i>u</i>)</span> is the sum of the numbers written on the edges on the path from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>.</p><p><span class="tex-font-style-it">Leaves</span> of a tree are vertices connected to a single vertex by a single edge, but the root of a tree is a <span class="tex-font-style-it">leaf</span> if and only if the tree consists of a single vertex&nbsp;— root.</p><p>Thus Alyona decided to remove some of tree leaves until there will be no any sad vertex left in the tree. What is the minimum number of leaves Alyona needs to remove?</p></div><div class="input-specification"><p>In the first line of the input integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) is given&nbsp;— the number of vertices in the tree.</p><p>In the second line the sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) is given, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number written on vertex <span class="tex-span"><i>i</i></span>.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines describe tree edges: <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them consists of two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, meaning that there is an edge connecting vertices <span class="tex-span"><i>i</i> + 1</span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> with number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> written on it.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the minimum number of leaves Alyona needs to remove such that there will be no any sad vertex left in the tree.</p></div>

## Input

<p>In the first line of the input integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) is given&nbsp;— the number of vertices in the tree.</p><p>In the second line the sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) is given, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number written on vertex <span class="tex-span"><i>i</i></span>.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines describe tree edges: <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them consists of two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, meaning that there is an edge connecting vertices <span class="tex-span"><i>i</i> + 1</span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> with number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> written on it.</p>

## Output

<p>Print the only integer&nbsp;— the minimum number of leaves Alyona needs to remove such that there will be no any sad vertex left in the tree.</p>





```input1
9
88 22 83 14 95 91 98 53 11
3 24
7 -8
1 67
1 64
9 65
5 12
6 -80
3 8

```




```output1
5

```



## Note

<p>The following image represents possible process of removing leaves from the tree: </p><center> <img class="tex-graphics" src="file://o3nViaPu.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
