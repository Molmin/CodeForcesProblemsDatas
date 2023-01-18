## Description

<div><p>For a permutation <span class="tex-span"><i>P</i>[1... <i>N</i>]</span> of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span>, function <span class="tex-span"><i>f</i></span> is defined as follows:</p><center> <img align="middle" class="tex-formula" src="file://b2fdKyxP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Let <span class="tex-span"><i>g</i>(<i>i</i>)</span> be the minimum positive integer <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>f</i>(<i>i</i>, <i>j</i>) = <i>i</i></span>. We can show such <span class="tex-span"><i>j</i></span> always exists.</p><p>For given <span class="tex-span"><i>N</i>, <i>A</i>, <i>B</i></span>, find a permutation <span class="tex-span"><i>P</i></span> of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span> such that for <span class="tex-span">1 ≤ <i>i</i> ≤ <i>N</i></span>, <span class="tex-span"><i>g</i>(<i>i</i>)</span> equals either <span class="tex-span"><i>A</i></span> or <span class="tex-span"><i>B</i></span>.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>N</i>, <i>A</i>, <i>B</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>A</i>, <i>B</i> ≤ <i>N</i></span>).</p></div><div class="output-specification"><p>If no such permutation exists, output <span class="tex-font-style-tt">-1</span>. Otherwise, output a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span>.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>N</i>, <i>A</i>, <i>B</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>A</i>, <i>B</i> ≤ <i>N</i></span>).</p>

## Output

<p>If no such permutation exists, output <span class="tex-font-style-tt">-1</span>. Otherwise, output a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span>.</p>





```input1
9 2 5

```




```input2
3 2 1

```




```output1
6 5 8 3 4 1 9 2 7
```




```output2
1 2 3
```



## Note

<p>In the first example, <span class="tex-span"><i>g</i>(1) = <i>g</i>(6) = <i>g</i>(7) = <i>g</i>(9) = 2</span> and <span class="tex-span"><i>g</i>(2) = <i>g</i>(3) = <i>g</i>(4) = <i>g</i>(5) = <i>g</i>(8) = 5</span> </p><p>In the second example, <span class="tex-span"><i>g</i>(1) = <i>g</i>(2) = <i>g</i>(3) = 1</span></p>
