## Description

<div><p>Recently Petya has become keen on physics. Anna V., his teacher noticed Petya's interest and gave him a fascinating physical puzzle — a half-decay tree. </p><p>A half-decay tree is a complete binary tree with the height <span class="tex-span"><i>h</i></span>. The height of a tree is the length of the path (in edges) from the root to a leaf in the tree. While studying the tree Petya can add electrons to vertices or induce random decay with synchrophasotron. Random decay is a process during which the edges of some path from the root to the random leaf of the tree are deleted. All the leaves are equiprobable. As the half-decay tree is the school property, Petya will return back the deleted edges into the tree after each decay.</p><p>After being desintegrated, the tree decomposes into connected components. Charge of each component is the total quantity of electrons placed in vertices of the component. Potential of desintegerated tree is the maximum from the charges of its connected components. Each time before inducing random decay Petya is curious about the mathematical expectation of potential of the tree after being desintegrated. </p></div><div class="input-specification"><p>First line will contain two integers <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 30, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>q</i></span> lines will contain a query of one of two types: </p><ul><li> <span class="tex-font-style-tt">add</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>e</i></span><p>Petya adds <span class="tex-span"><i>e</i></span> electrons to vertex number <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ 2<sup class="upper-index"><i>h</i> + 1</sup> - 1, 0 ≤ <i>e</i> ≤ 10<sup class="upper-index">4</sup></span>). <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>e</i></span> are integers.</p><p>The vertices of the tree are numbered in the following way: the root is numbered with 1, the children of the vertex with number <span class="tex-span"><i>x</i></span> are numbered with <span class="tex-span">2<i>x</i></span> and <span class="tex-span">2<i>x</i> + 1</span>.</p></li><li> <span class="tex-font-style-tt">decay</span><p>Petya induces tree decay. </p></li></ul></div><div class="output-specification"><p>For each query <span class="tex-font-style-tt">decay</span> solution you should output the mathematical expectation of potential of the tree after being desintegrated. The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>First line will contain two integers <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 30, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>q</i></span> lines will contain a query of one of two types: </p><ul><li> <span class="tex-font-style-tt">add</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>e</i></span><p>Petya adds <span class="tex-span"><i>e</i></span> electrons to vertex number <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ 2<sup class="upper-index"><i>h</i> + 1</sup> - 1, 0 ≤ <i>e</i> ≤ 10<sup class="upper-index">4</sup></span>). <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>e</i></span> are integers.</p><p>The vertices of the tree are numbered in the following way: the root is numbered with 1, the children of the vertex with number <span class="tex-span"><i>x</i></span> are numbered with <span class="tex-span">2<i>x</i></span> and <span class="tex-span">2<i>x</i> + 1</span>.</p></li><li> <span class="tex-font-style-tt">decay</span><p>Petya induces tree decay. </p></li></ul>

## Output

<p>For each query <span class="tex-font-style-tt">decay</span> solution you should output the mathematical expectation of potential of the tree after being desintegrated. The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
1 4
add 1 3
add 2 10
add 3 11
decay

```




```output1
13.50000000

```


