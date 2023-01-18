## Description

<div><p>We'll define <span class="tex-span"><i>S</i>(<i>n</i>)</span> for positive integer <span class="tex-span"><i>n</i></span> as follows: the number of the <span class="tex-span"><i>n</i></span>'s digits in the decimal base. For example, <span class="tex-span"><i>S</i>(893) = 3</span>, <span class="tex-span"><i>S</i>(114514) = 6</span>.</p><p>You want to make a consecutive integer sequence starting from number <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i>, <i>m</i> + 1, ...</span>). But you need to pay <span class="tex-span"><i>S</i>(<i>n</i>)·<i>k</i></span> to add the number <span class="tex-span"><i>n</i></span> to the sequence.</p><p>You can spend a cost up to <span class="tex-span"><i>w</i></span>, and you want to make the sequence as long as possible. Write a program that tells sequence's maximum length.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">16</sup></span>), <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">16</sup></span>), <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>The first line should contain a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">16</sup></span>), <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">16</sup></span>), <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>The first line should contain a single integer — the answer to the problem.</p>





```input1
9 1 1

```




```input2
77 7 7

```




```input3
114 5 14

```




```input4
1 1 2

```




```output1
9

```




```output2
7

```




```output3
6

```




```output4
0

```


