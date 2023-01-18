## Description

<div><p>A tree is a connected graph without cycles.</p><p>Two trees, consisting of <span class="tex-span"><i>n</i></span> vertices each, are called <span class="tex-font-style-it">isomorphic</span> if there exists a permutation <span class="tex-span"><i>p</i>: {1, ..., <i>n</i>} → {1, ..., <i>n</i>}</span> such that the edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span> is present in the first tree if and only if the edge <span class="tex-span">(<i>p</i><sub class="lower-index"><i>u</i></sub>, <i>p</i><sub class="lower-index"><i>v</i></sub>)</span> is present in the second tree.</p><p>Vertex of the tree is called internal if its degree is greater than or equal to two.</p><p>Count the number of different non-isomorphic trees, consisting of <span class="tex-span"><i>n</i></span> vertices, such that the degree of each internal vertex is <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>d</i></span>. Print the answer over the given prime modulo <span class="tex-span"><i>mod</i></span>.</p></div><div class="input-specification"><p>The single line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and&nbsp;<span class="tex-span"><i>mod</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">2 ≤ <i>d</i> ≤ 10</span>, <span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— the number of vertices in the tree, the degree of internal vertices and the prime modulo.</p></div><div class="output-specification"><p>Print the number of trees over the modulo <span class="tex-span"><i>mod</i></span>.</p></div>

## Input

<p>The single line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and&nbsp;<span class="tex-span"><i>mod</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">2 ≤ <i>d</i> ≤ 10</span>, <span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— the number of vertices in the tree, the degree of internal vertices and the prime modulo.</p>

## Output

<p>Print the number of trees over the modulo <span class="tex-span"><i>mod</i></span>.</p>





```input1
5 2 433416647

```




```input2
10 3 409693891

```




```input3
65 4 177545087

```




```output1
1

```




```output2
2

```




```output3
910726

```


