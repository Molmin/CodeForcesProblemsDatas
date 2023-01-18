## Description

<div><p>You are given a positive integer <span class="tex-span"><i>n</i></span>. Let's build a graph on vertices <span class="tex-span">1, 2, ..., <i>n</i></span> in such a way that there is an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> if and only if <img align="middle" class="tex-formula" src="file://mnSAIC6n.png" style="max-width: 100.0%;max-height: 100.0%;">. Let <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> be the shortest distance between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, or <span class="tex-span">0</span> if there is no path between them. Compute the sum of values <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> over all <span class="tex-span">1 ≤ <i>u</i> &lt; <i>v</i> ≤ <i>n</i></span>.</p><p>The <span class="tex-span"><i>gcd</i></span> (greatest common divisor) of two positive integers is the maximum positive integer that divides both of the integers.</p></div><div class="input-specification"><p>Single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print the sum of <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> over all <span class="tex-span">1 ≤ <i>u</i> &lt; <i>v</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>Single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print the sum of <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> over all <span class="tex-span">1 ≤ <i>u</i> &lt; <i>v</i> ≤ <i>n</i></span>.</p>





```input1
6

```




```input2
10

```




```output1
8

```




```output2
44

```



## Note

<p>All shortest paths in the first example: </p><ul> <li> <img align="middle" class="tex-formula" src="file://MOo85NTf.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://AvRdiA87.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://sz395VhY.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://UlYMYORk.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://MxL4ib7M.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://VliRWDzA.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul><p>There are no paths between other pairs of vertices.</p><p>The total distance is <span class="tex-span">2 + 1 + 1 + 2 + 1 + 1 = 8</span>.</p>
