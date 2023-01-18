## Description

<div><p><span class="tex-font-style-it">Just in case somebody missed it: we have wonderful girls in Arpa’s land.</span></p><p>Arpa has a rooted tree (connected acyclic graph) consisting of <span class="tex-span"><i>n</i></span> vertices. The vertices are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>, the vertex <span class="tex-span">1</span> is the root. There is a letter written on each edge of this tree. Mehrdad is a fan of <span class="tex-font-style-it">Dokhtar-kosh</span> things. He call a string Dokhtar-kosh, if we can shuffle the characters in string such that it becomes palindrome.</p><center> <img class="tex-graphics" height="222px" src="file://gkFPEhXN.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center><p>He asks Arpa, for each vertex <span class="tex-span"><i>v</i></span>, what is the length of the longest simple path in subtree of <span class="tex-span"><i>v</i></span> that form a Dokhtar-kosh string.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree.</p><p><span class="tex-span">(<i>n</i>  -  1)</span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them contain an integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and a letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> (<span class="tex-span">1  ≤  <i>p</i><sub class="lower-index"><i>i</i> + 1</sub>  ≤  <i>i</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> is lowercase English letter, between <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">v</span>, inclusively), that mean that there is an edge between nodes <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and <span class="tex-span"><i>i</i> + 1</span> and there is a letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> written on this edge.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be the length of the longest simple path in subtree of the <span class="tex-span"><i>i</i></span>-th vertex that form a Dokhtar-kosh string.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree.</p><p><span class="tex-span">(<i>n</i>  -  1)</span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them contain an integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and a letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> (<span class="tex-span">1  ≤  <i>p</i><sub class="lower-index"><i>i</i> + 1</sub>  ≤  <i>i</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> is lowercase English letter, between <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">v</span>, inclusively), that mean that there is an edge between nodes <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and <span class="tex-span"><i>i</i> + 1</span> and there is a letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> written on this edge.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be the length of the longest simple path in subtree of the <span class="tex-span"><i>i</i></span>-th vertex that form a Dokhtar-kosh string.</p>





```input1
4
1 s
2 a
3 s

```




```input2
5
1 a
2 h
1 a
4 h

```




```output1
3 1 1 0
```




```output2
4 1 0 1 0
```


