## Description

<div><p>The graph is called <span class="tex-font-style-it">tree</span> if it is connected and has no cycles. Suppose the tree is rooted at some vertex. Then tree is called to be perfect $k$-ary tree if each vertex is either a leaf (has no children) or has exactly $k$ children. Also, in perfect $k$-ary tree all leafs must have same depth.</p><p>For example, the picture below illustrates perfect binary tree with $15$ vertices:</p><center><img class="tex-graphics" src="file://9MZAqa6X.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>There is a perfect $k$-ary tree with $n$ nodes. The nodes are labeled with distinct integers from $1$ to $n$, however you don't know how nodes are labelled. Still, you want to find the label of the root of the tree.</p><p>You are allowed to make at most $60 \cdot n$ queries of the following type:</p><ul> <li> "<span class="tex-font-style-tt">? $a$ $b$ $c$</span>", the query returns "<span class="tex-font-style-tt">Yes</span>" if node with label $b$ lies on the path from $a$ to $c$ and "<span class="tex-font-style-tt">No</span>" otherwise. </li></ul><p>Both $a$ and $c$ are considered to be lying on the path from $a$ to $c$.</p><p>When you are ready to report the root of the tree, print </p><ul> <li> "<span class="tex-font-style-tt">! $s$</span>", where $s$ is the label of the root of the tree. </li></ul><p>It is possible to report the root only once and this query is not counted towards limit of $60 \cdot n$ queries.</p></div><div><h2>Interaction</h2><p>The first line of the standard input stream contains two integers $n$ and $k$ ($3 \le n \le 1500$, $2 \le k &lt; n$)&nbsp;— the number of nodes in the tree and the value of $k$. </p><p>It is guaranteed that $n$ is such that the tree forms a perfect $k$-ary tree.</p><p>You can ask at most $60 \cdot n$ queries. To ask a query, print a line of form "<span class="tex-font-style-tt">? $a$ $b$ $c$</span>", where $1 \le a, b, c \le n$. After that you should read a single line containing "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">No</span>" depending on the answer of the query.</p><p>The tree is fixed for each test and it doesn't depend on your queries.</p><p>When you are ready to print the answer, print a line of the form "<span class="tex-font-style-tt">! $s$</span>", where $s$ is the label of the root vertex and then terminate your program.</p><p>After printing each query do not forget to print end of line and flush the output. Otherwise you may get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> See documentation for other languages.</li></ul><p>In case your program will make more than $60 \cdot n$ queries, but in other aspects would follow the interaction protocol and terminate coorectly, it will get verdict «<span class="tex-font-style-tt">Wrong Answer</span>».</p><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack the solution use the following test format:</p><p>The first line should contain integers $n$ and $k$ ($3 \le n \le 1500$, $2 \le k \le 1500$)&nbsp;— the number of vertices and the $k$ parameter of the tree.</p><p>Of course, the value of $n$ must correspond to the size of the valid $k$-ary tree of some depth.</p><p>The second line should contain $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the labels of the tree in the natural order, all labels must be distinct.</p><p>Let's call the following ordering of the tree vertices to be natural: first the root of the tree goes, then go all vertices on depth of one edge from root, ordered from left to right, then go all vertices on depth of two edges from root, ordered from left to right, and so on until the maximum depth.</p><p>This way, the $a_1$ is the answer for the hack.</p></div>





```input1
3 2

No

Yes

```




```output1
? 1 3 2

? 1 2 3

! 2
```



## Note

<p>The tree in the example is as follows:</p><center><img class="tex-graphics" src="file://Hy0gYbl2.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The input and output for example illustrate possible interaction on that test (empty lines are inserted only for clarity).</p><p>The hack corresponding to the example would look like:</p><pre class="verbatim"><br>3 2<br>2 3 1<br></pre>
