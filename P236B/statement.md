## Description

<div><p>Let's denote <span class="tex-span"><i>d</i>(<i>n</i>)</span> as the number of divisors of a positive integer <span class="tex-span"><i>n</i></span>. You are given three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>. Your task is to calculate the following sum:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://2Yb8LOtd.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Find the sum modulo <span class="tex-span">1073741824</span> <span class="tex-span">(2<sup class="upper-index">30</sup>)</span>.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print a single integer — the required sum modulo <span class="tex-span">1073741824</span> <span class="tex-span">(2<sup class="upper-index">30</sup>)</span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 100</span>).</p>

## Output

<p>Print a single integer — the required sum modulo <span class="tex-span">1073741824</span> <span class="tex-span">(2<sup class="upper-index">30</sup>)</span>.</p>





```input1
2 2 2

```




```input2
5 6 7

```




```output1
20

```




```output2
1520

```



## Note

<p>For the first example.</p><ul> <li> <span class="tex-span"><i>d</i>(1·1·1) = <i>d</i>(1) = 1</span>; </li><li> <span class="tex-span"><i>d</i>(1·1·2) = <i>d</i>(2) = 2</span>; </li><li> <span class="tex-span"><i>d</i>(1·2·1) = <i>d</i>(2) = 2</span>; </li><li> <span class="tex-span"><i>d</i>(1·2·2) = <i>d</i>(4) = 3</span>; </li><li> <span class="tex-span"><i>d</i>(2·1·1) = <i>d</i>(2) = 2</span>; </li><li> <span class="tex-span"><i>d</i>(2·1·2) = <i>d</i>(4) = 3</span>; </li><li> <span class="tex-span"><i>d</i>(2·2·1) = <i>d</i>(4) = 3</span>; </li><li> <span class="tex-span"><i>d</i>(2·2·2) = <i>d</i>(8) = 4</span>. </li></ul><p>So the result is <span class="tex-span">1 + 2 + 2 + 3 + 2 + 3 + 3 + 4 = 20</span>.</p>
