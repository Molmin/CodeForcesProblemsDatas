## Description

<div><p>Let <span class="tex-span"><i>S</i>(<i>n</i>)</span> denote the number that represents the digits of <span class="tex-span"><i>n</i></span> in sorted order. For example, <span class="tex-span"><i>S</i>(1) = 1, <i>S</i>(5) = 5, <i>S</i>(50394) = 3459, <i>S</i>(353535) = 333555</span>.</p><p>Given a number <span class="tex-span"><i>X</i></span>, compute <img align="middle" class="tex-formula" src="file://SuU3gv5A.png" style="max-width: 100.0%;max-height: 100.0%;"> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input will contain the integer <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>X</i> ≤ 10<sup class="upper-index">700</sup></span>).</p></div><div class="output-specification"><p>Print a single integer, the answer to the question.</p></div>

## Input

<p>The first line of input will contain the integer <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>X</i> ≤ 10<sup class="upper-index">700</sup></span>).</p>

## Output

<p>Print a single integer, the answer to the question.</p>





```input1
21

```




```input2
345342

```




```output1
195

```




```output2
390548434

```



## Note

<p>The first few values of <span class="tex-span"><i>S</i></span> are <span class="tex-span">1, 2, 3, 4, 5, 6, 7, 8, 9, 1, 11, 12, 13, 14, 15, 16, 17, 18, 19, 2, 12</span>. The sum of these values is <span class="tex-span">195</span>. </p>
