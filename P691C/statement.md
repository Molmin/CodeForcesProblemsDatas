## Description

<div><p>You are given a positive decimal number <span class="tex-span"><i>x</i></span>.</p><p>Your task is to convert it to the "<span class="tex-font-style-tt">simple exponential notation</span>".</p><p>Let <span class="tex-span"><i>x</i> = <i>a</i>·10<sup class="upper-index"><i>b</i></sup></span>, where <span class="tex-span">1 ≤ <i>a</i> &lt; 10</span>, then in general case the "<span class="tex-font-style-tt">simple exponential notation</span>" looks like "<span class="tex-font-style-tt">aEb</span>". If <span class="tex-span"><i>b</i></span> equals to zero, the part "<span class="tex-font-style-tt">Eb</span>" should be skipped. If <span class="tex-span"><i>a</i></span> is an integer, it should be written without decimal point. Also there should not be extra zeroes in <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The only line contains the positive decimal number <span class="tex-span"><i>x</i></span>. The length of the line will not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. Note that you are given too large number, so you can't use standard built-in data types "<span class="tex-font-style-tt">float</span>", "<span class="tex-font-style-tt">double</span>" and other.</p></div><div class="output-specification"><p>Print the only line — the "<span class="tex-font-style-tt">simple exponential notation</span>" of the given number <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The only line contains the positive decimal number <span class="tex-span"><i>x</i></span>. The length of the line will not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. Note that you are given too large number, so you can't use standard built-in data types "<span class="tex-font-style-tt">float</span>", "<span class="tex-font-style-tt">double</span>" and other.</p>

## Output

<p>Print the only line — the "<span class="tex-font-style-tt">simple exponential notation</span>" of the given number <span class="tex-span"><i>x</i></span>.</p>





```input1
16

```




```input2
01.23400

```




```input3
.100

```




```input4
100.

```




```output1
1.6E1

```




```output2
1.234

```




```output3
1E-1

```




```output4
1E2

```


