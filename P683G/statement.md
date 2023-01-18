## Description

<div><p>Periodic decimal fraction is usually written as: <span class="tex-font-style-tt">[entire_part.non-periodic_part (period)]</span>. Any simple fraction can be represented as a periodic decimal fraction and vice versa. For example, the decimal fraction <span class="tex-span">0.2(45)</span> corresponds to a fraction <span class="tex-span">27 / 110</span>. Your task is to convert the periodic fraction to a simple periodic fraction.</p></div><div class="input-specification"><p>The first line contains the periodic decimal fraction <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 &lt; <i>x</i> &lt; 1</span>) in the format described in the statement. The total number of digits in the period and non-periodic part of the fraction does not exceed 8. Non-periodic part may be absent, the periodic part can't be absent (but it can be equal to any non-negative number).</p></div><div class="output-specification"><p>Print the representation of the fraction <span class="tex-span"><i>x</i></span> as a simple fraction <span class="tex-span"><i>p</i> / <i>q</i></span>, where <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are mutually prime integers.</p></div>

## Input

<p>The first line contains the periodic decimal fraction <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 &lt; <i>x</i> &lt; 1</span>) in the format described in the statement. The total number of digits in the period and non-periodic part of the fraction does not exceed 8. Non-periodic part may be absent, the periodic part can't be absent (but it can be equal to any non-negative number).</p>

## Output

<p>Print the representation of the fraction <span class="tex-span"><i>x</i></span> as a simple fraction <span class="tex-span"><i>p</i> / <i>q</i></span>, where <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are mutually prime integers.</p>





```input1
0.2(45)

```




```input2
0.75(0)

```




```output1
27/110

```




```output2
3/4

```


