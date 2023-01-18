## Description

<div><p>Greatest common divisor <span class="tex-span"><i>GCD</i>(<i>a</i>, <i>b</i>)</span> of two positive integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is equal to the biggest integer <span class="tex-span"><i>d</i></span> such that both integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are divisible by <span class="tex-span"><i>d</i></span>. There are many efficient algorithms to find greatest common divisor <span class="tex-span"><i>GCD</i>(<i>a</i>, <i>b</i>)</span>, for example, Euclid algorithm. </p><p>Formally, find the biggest integer <span class="tex-span"><i>d</i></span>, such that all integers <span class="tex-span"><i>a</i>, <i>a</i> + 1, <i>a</i> + 2, ..., <i>b</i></span> are divisible by <span class="tex-span"><i>d</i></span>. To make the problem even more complicated we allow <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> to be up to googol, <span class="tex-span">10<sup class="upper-index">100</sup></span>&nbsp;— such number do not fit even in 64-bit integer type!</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">100</sup></span>).</p></div><div class="output-specification"><p>Output one integer&nbsp;— greatest common divisor of all integers from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> inclusive.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">100</sup></span>).</p>

## Output

<p>Output one integer&nbsp;— greatest common divisor of all integers from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> inclusive.</p>





```input1
1 2

```




```input2
61803398874989484820458683436563811772030917980576 61803398874989484820458683436563811772030917980576

```




```output1
1

```




```output2
61803398874989484820458683436563811772030917980576

```


