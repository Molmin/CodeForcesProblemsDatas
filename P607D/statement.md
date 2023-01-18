## Description

<div><p>Genos and Saitama went shopping for Christmas trees. However, a different type of tree caught their attention, the exalted Power Tree. </p><p>A Power Tree starts out as a single root vertex indexed <span class="tex-span">1</span>. A Power Tree grows through a magical phenomenon known as an update. In an <span class="tex-font-style-it">update</span>, a single vertex is added to the tree as a child of some other vertex.</p><p>Every vertex in the tree (the root and all the added vertices) has some value <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> associated with it. The <span class="tex-font-style-it">power</span> of a vertex is defined as the strength of the multiset composed of the value associated with this vertex (<span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>) and the <span class="tex-font-style-it">powers</span> of its direct children. The <span class="tex-font-style-it">strength</span> of a multiset is defined as the sum of all elements in the <span class="tex-font-style-bf">multiset</span> multiplied by the number of elements in it. Or in other words for some <span class="tex-font-style-bf">multiset</span> <span class="tex-span"><i>S</i></span>: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://2vSnLN4I.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Saitama knows the <span class="tex-font-style-it">updates</span> that will be performed on the tree, so he decided to test Genos by asking him queries about the tree during its growth cycle.</p><p>An update is of the form <span class="tex-span">1&nbsp;<i>p</i>&nbsp;<i>v</i></span>, and adds a new vertex with value <span class="tex-span"><i>v</i></span> as a child of vertex <span class="tex-span"><i>p</i></span>.</p><p>A query is of the form <span class="tex-span">2&nbsp;<i>u</i></span>, and asks for the power of vertex <span class="tex-span"><i>u</i></span>.</p><p>Please help Genos respond to these queries modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains two space separated integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub> &lt; 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>) — the value of vertex <span class="tex-span">1</span> and the total number of updates and queries respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the updates and queries. Each of them has one of the following forms: </p><ul> <li> <span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>v</i><sub class="lower-index"><i>i</i></sub></span>, if these line describes an update. The index of the added vertex is equal to the smallest positive integer not yet used as an index in the tree. It is guaranteed that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is some already existing vertex and <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">9</sup></span>. </li><li> <span class="tex-span">2&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub></span>, if these line describes a query. It is guaranteed <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> will exist in the tree. </li></ul><p>It is guaranteed that the input will contain at least one query.</p></div><div class="output-specification"><p>For each query, print out the power of the given vertex modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains two space separated integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub> &lt; 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>) — the value of vertex <span class="tex-span">1</span> and the total number of updates and queries respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the updates and queries. Each of them has one of the following forms: </p><ul> <li> <span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>v</i><sub class="lower-index"><i>i</i></sub></span>, if these line describes an update. The index of the added vertex is equal to the smallest positive integer not yet used as an index in the tree. It is guaranteed that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is some already existing vertex and <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">9</sup></span>. </li><li> <span class="tex-span">2&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub></span>, if these line describes a query. It is guaranteed <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> will exist in the tree. </li></ul><p>It is guaranteed that the input will contain at least one query.</p>

## Output

<p>For each query, print out the power of the given vertex modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 5
1 1 3
1 2 5
1 3 7
1 4 11
2 1

```




```input2
5 5
1 1 4
1 2 3
2 2
1 2 7
2 1

```




```output1
344

```




```output2
14
94

```



## Note

<p>For the first sample case, after all the updates the graph will have vertices labelled in the following manner: 1 — 2 — 3 — 4 — 5</p><p>These vertices will have corresponding values: 2 — 3 — 5 — 7 — 11</p><p>And corresponding powers: 344 — 170 — 82 — 36 — 11</p>
