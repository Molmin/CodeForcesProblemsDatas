## Description

<div><p>A little girl loves problems on bitwise operations very much. Here's one of them.</p><p>You are given two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. Let's consider the values of <img align="middle" class="tex-formula" src="file://DFXZbEHu.png" style="max-width: 100.0%;max-height: 100.0%;"> for all pairs of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>l</i> ≤ <i>a</i> ≤ <i>b</i> ≤ <i>r</i>)</span>. Your task is to find the maximum value among all considered ones.</p><p>Expression <img align="middle" class="tex-formula" src="file://pit7v79M.png" style="max-width: 100.0%;max-height: 100.0%;"> means applying bitwise excluding or operation to integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. The given operation exists in all modern programming languages, for example, in languages <span class="tex-span"><i>C</i></span>++ and <span class="tex-span"><i>Java</i></span> it is represented as "<span class="tex-font-style-tt">^</span>", in <span class="tex-span"><i>Pascal</i></span> — as "<span class="tex-font-style-tt">xor</span>".</p></div><div class="input-specification"><p>The single line contains space-separated integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>In a single line print a single integer — the maximum value of <img align="middle" class="tex-formula" src="file://CL9ZcDKN.png" style="max-width: 100.0%;max-height: 100.0%;"> for all pairs of integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>l</i> ≤ <i>a</i> ≤ <i>b</i> ≤ <i>r</i>)</span>.</p></div>

## Input

<p>The single line contains space-separated integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>In a single line print a single integer — the maximum value of <img align="middle" class="tex-formula" src="file://CL9ZcDKN.png" style="max-width: 100.0%;max-height: 100.0%;"> for all pairs of integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>l</i> ≤ <i>a</i> ≤ <i>b</i> ≤ <i>r</i>)</span>.</p>





```input1
1 2

```




```input2
8 16

```




```input3
1 1

```




```output1
3

```




```output2
31

```




```output3
0

```


