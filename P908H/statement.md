## Description

<div><p>Your friend has a hidden directed graph with <span class="tex-span"><i>n</i></span> nodes.</p><p>Let <span class="tex-span"><i>f</i>(<i>u</i>, <i>v</i>)</span> be true if there is a directed path from node <span class="tex-span"><i>u</i></span> to node <span class="tex-span"><i>v</i></span>, and false otherwise. For each pair of distinct nodes, <span class="tex-span"><i>u</i>, <i>v</i></span>, you know at least one of the three statements is true: </p><ol> <li> <img align="middle" class="tex-formula" src="file://aObYRJzg.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://g2EIy4OE.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://xwfBVlx1.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ol><p>Here AND, OR and XOR mean AND, OR and exclusive OR operations, respectively.</p><p>You are given an <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>n</i></span> matrix saying which one of the three statements holds for each pair of vertices. The entry in the <span class="tex-span"><i>u</i></span>-th row and <span class="tex-span"><i>v</i></span>-th column has a single character. </p><ol> <li> If the first statement holds, this is represented by the character '<span class="tex-font-style-tt">A</span>'. </li><li> If the second holds, this is represented by the character '<span class="tex-font-style-tt">O</span>'. </li><li> If the third holds, this is represented by the character '<span class="tex-font-style-tt">X</span>'. </li><li> The diagonal of this matrix will only contain the character '<span class="tex-font-style-tt">-</span>'. </li></ol><p>Note that it is possible that a pair of nodes may satisfy multiple statements, in which case, the character given will represent one of the true statements for that pair. This matrix is also guaranteed to be symmetric.</p><p>You would like to know if there is a directed graph that is consistent with this matrix. If it is impossible, print the integer <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum number of edges that could be consistent with this information.</p></div><div class="input-specification"><p>The first line will contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 47</span>), the number of nodes.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain <span class="tex-span"><i>n</i></span> characters each: the matrix of what you know about the graph connectivity in the format described in the statement.</p></div><div class="output-specification"><p>Print the minimum number of edges that is consistent with the given information, or <span class="tex-font-style-tt">-1</span> if it is impossible.</p></div>

## Input

<p>The first line will contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 47</span>), the number of nodes.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain <span class="tex-span"><i>n</i></span> characters each: the matrix of what you know about the graph connectivity in the format described in the statement.</p>

## Output

<p>Print the minimum number of edges that is consistent with the given information, or <span class="tex-font-style-tt">-1</span> if it is impossible.</p>





```input1
4
-AAA
A-AA
AA-A
AAA-

```




```input2
3
-XX
X-X
XX-

```




```output1
4

```




```output2
2

```



## Note

<p>Sample 1: The hidden graph is a strongly connected graph. We can put all four nodes in a cycle.</p><p>Sample 2: One valid graph is <span class="tex-span">3 → 1 → 2</span>. For each distinct pair, exactly one of <span class="tex-span"><i>f</i>(<i>u</i>, <i>v</i>), <i>f</i>(<i>v</i>, <i>u</i>)</span> holds.</p>
