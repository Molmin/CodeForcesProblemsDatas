## Description

<div><p>For a given positive integer <span class="tex-span"><i>n</i></span> denote its <span class="tex-span"><i>k</i></span>-rounding as the minimum positive integer <span class="tex-span"><i>x</i></span>, such that <span class="tex-span"><i>x</i></span> ends with <span class="tex-span"><i>k</i></span> or more zeros in base <span class="tex-span">10</span> and is divisible by <span class="tex-span"><i>n</i></span>.</p><p>For example, <span class="tex-span">4</span>-rounding of <span class="tex-span">375</span> is <span class="tex-span">375·80 = 30000</span>. <span class="tex-span">30000</span> is the minimum integer such that it ends with <span class="tex-span">4</span> or more zeros and is divisible by <span class="tex-span">375</span>.</p><p>Write a program that will perform the <span class="tex-span"><i>k</i></span>-rounding of <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 8</span>).</p></div><div class="output-specification"><p>Print the <span class="tex-span"><i>k</i></span>-rounding of <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 8</span>).</p>

## Output

<p>Print the <span class="tex-span"><i>k</i></span>-rounding of <span class="tex-span"><i>n</i></span>.</p>





```input1
375 4

```




```input2
10000 1

```




```input3
38101 0

```




```input4
123456789 8

```




```output1
30000

```




```output2
10000

```




```output3
38101

```




```output4
12345678900000000

```


