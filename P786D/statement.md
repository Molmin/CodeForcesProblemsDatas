## Description

<div><p>Rick is in love with Unity. But Mr. Meeseeks also love Unity, so Rick and Mr. Meeseeks are "love rivals". </p><p>Unity loves rap, so it decided that they have to compete in a rap game (battle) in order to choose the best. Rick is too nerds, so instead he's gonna make his verse with running his original algorithm on lyrics "Rap God" song.</p><center> <img class="tex-graphics" src="file://bqqKlygG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>His algorithm is a little bit complicated. He's made a tree with <span class="tex-span"><i>n</i></span> vertices numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and there's a lowercase english letter written on each edge. He denotes <span class="tex-span"><i>str</i>(<i>a</i>, <i>b</i>)</span> to be the string made by writing characters on edges on the shortest path from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> one by one (a string of length equal to distance of <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>). Note that <span class="tex-span"><i>str</i>(<i>a</i>, <i>b</i>)</span> is reverse of <span class="tex-span"><i>str</i>(<i>b</i>, <i>a</i>)</span> and <span class="tex-span"><i>str</i>(<i>a</i>, <i>a</i>)</span> is empty.</p><p> In order to make the best verse he can, he needs to answer some queries, but he's not a computer scientist and is not able to answer those queries, so he asked you to help him. Each query is characterized by two vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> ≠ <i>y</i></span>). Answer to this query is the number of vertices like <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>z</i> ≠ <i>x</i>, <i>z</i> ≠ <i>y</i></span> and <span class="tex-span"><i>str</i>(<i>x</i>, <i>y</i>)</span> is lexicographically larger than <span class="tex-span"><i>str</i>(<i>x</i>, <i>z</i>)</span>.</p><p>String <span class="tex-span"><i>x</i>  =  <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>...<i>x</i><sub class="lower-index">|<i>x</i>|</sub></span> is lexicographically larger than string <span class="tex-span"><i>y</i>  =  <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>...<i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, if either <span class="tex-span">|<i>x</i>|  &gt;  |<i>y</i>|</span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>  =  <i>y</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">2</sub>  =  <i>y</i><sub class="lower-index">2</sub>,  ...,  <i>x</i><sub class="lower-index">|<i>y</i>|</sub>  =  <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, or exists such number <span class="tex-span"><i>r</i> (<i>r</i>  &lt;  |<i>x</i>|,  <i>r</i>  &lt;  |<i>y</i>|)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>  =  <i>y</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">2</sub>  =  <i>y</i><sub class="lower-index">2</sub>,  ...,  <i>x</i><sub class="lower-index"><i>r</i></sub>  =  <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i>  +  1</sub>  &gt;  <i>y</i><sub class="lower-index"><i>r</i>  +  1</sub></span>. Characters are compared like their ASCII codes (or alphabetic order).</p><p>Help Rick get the girl (or whatever gender Unity has).</p></div><div class="input-specification"><p>The first line of input contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 20000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 20000</span>) — number of vertices in tree and number of queries respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the edges. Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (endpoints of the edge) followed by an English lowercase letter <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>, <i>v</i> ≠ <i>u</i></span>).</p><p>The next <span class="tex-span"><i>q</i></span> line contain the queries. Each line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>).</p></div><div class="output-specification"><p>Print the answer for each query in one line.</p></div>

## Input

<p>The first line of input contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 20000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 20000</span>) — number of vertices in tree and number of queries respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the edges. Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (endpoints of the edge) followed by an English lowercase letter <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>, <i>v</i> ≠ <i>u</i></span>).</p><p>The next <span class="tex-span"><i>q</i></span> line contain the queries. Each line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>).</p>

## Output

<p>Print the answer for each query in one line.</p>





```input1
4 3
4 1 t
3 2 p
1 2 s
3 2
1 3
2 1

```




```input2
8 4
4 6 p
3 7 o
7 8 p
4 5 d
1 3 o
4 3 p
3 2 e
8 6
3 7
8 1
4 3

```




```output1
0
1
1

```




```output2
6
1
3
1

```



## Note

<p>Here's the tree of first sample testcase:</p><center> <img class="tex-graphics" src="file://scC86uEu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Here's the tree of second sample testcase:</p><center> <img class="tex-graphics" src="file://Y1e8e8m8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In this test:</p><ul> <li> <span class="tex-span"><i>str</i>(8, 1)</span> = <span class="tex-font-style-tt">poo</span> </li><li> <span class="tex-span"><i>str</i>(8, 2)</span> = <span class="tex-font-style-tt">poe</span> </li><li> <span class="tex-span"><i>str</i>(8, 3)</span> = <span class="tex-font-style-tt">po</span> </li><li> <span class="tex-span"><i>str</i>(8, 4)</span> = <span class="tex-font-style-tt">pop</span> </li><li> <span class="tex-span"><i>str</i>(8, 5)</span> = <span class="tex-font-style-tt">popd</span> </li><li> <span class="tex-span"><i>str</i>(8, 6)</span> = <span class="tex-font-style-tt">popp</span> </li><li> <span class="tex-span"><i>str</i>(8, 7)</span> = <span class="tex-font-style-tt">p</span> </li></ul><p>So, for the first query, <img align="middle" class="tex-formula" src="file://qWpgt3GL.png" style="max-width: 100.0%;max-height: 100.0%;"> and for the third query <img align="middle" class="tex-formula" src="file://NmdrBifS.png" style="max-width: 100.0%;max-height: 100.0%;"> is the answer.</p>
