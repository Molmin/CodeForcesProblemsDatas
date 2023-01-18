## Description

<div><p>Count the number of distinct sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>) consisting of positive integers such that <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>) = <i>x</i></span> and <img align="middle" class="tex-formula" src="file://pAGAjdpF.png" style="max-width: 100.0%;max-height: 100.0%;">. As this number could be large, print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p><span class="tex-span"><i>gcd</i></span> here means the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a>.</p></div><div class="input-specification"><p>The only line contains two positive integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the number of such sequences modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line contains two positive integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the number of such sequences modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 9

```




```input2
5 8

```




```output1
3

```




```output2
0

```



## Note

<p>There are three suitable sequences in the first test: <span class="tex-span">(3, 3, 3)</span>, <span class="tex-span">(3, 6)</span>, <span class="tex-span">(6, 3)</span>.</p><p>There are no suitable sequences in the second test.</p>
