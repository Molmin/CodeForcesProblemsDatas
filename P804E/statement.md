## Description

<div><p>Seyyed and MoJaK are friends of Sajjad. Sajjad likes a permutation. Seyyed wants to change the permutation in a way that Sajjad won't like it. Seyyed thinks more swaps yield more probability to do that, so he makes MoJaK to perform a swap between every pair of positions <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, where <span class="tex-span"><i>i</i> &lt; <i>j</i></span>, exactly once. MoJaK doesn't like to upset Sajjad.</p><p>Given the permutation, determine whether it is possible to swap all pairs of positions so that the permutation stays the same. If it is possible find how to do that. </p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the size of the permutation.</p><p>As the permutation is not important, you can consider <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>, where the permutation is <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p></div><div class="output-specification"><p>If it is not possible to swap all pairs of positions so that the permutation stays the same, print "<span class="tex-font-style-tt">NO</span>",</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>", then print <img align="middle" class="tex-formula" src="file://xoR5Oa5M.png" style="max-width: 100.0%;max-height: 100.0%;"> lines: the <span class="tex-span"><i>i</i></span>-th of these lines should contain two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> &lt; <i>b</i></span>)&nbsp;— the positions where the <span class="tex-span"><i>i</i></span>-th swap is performed.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the size of the permutation.</p><p>As the permutation is not important, you can consider <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>, where the permutation is <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p>

## Output

<p>If it is not possible to swap all pairs of positions so that the permutation stays the same, print "<span class="tex-font-style-tt">NO</span>",</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>", then print <img align="middle" class="tex-formula" src="file://xoR5Oa5M.png" style="max-width: 100.0%;max-height: 100.0%;"> lines: the <span class="tex-span"><i>i</i></span>-th of these lines should contain two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> &lt; <i>b</i></span>)&nbsp;— the positions where the <span class="tex-span"><i>i</i></span>-th swap is performed.</p>





```input1
3

```




```input2
1

```




```output1
NO

```




```output2
YES

```


