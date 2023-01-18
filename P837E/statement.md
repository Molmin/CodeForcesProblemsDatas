## Description

<div><p>Vasya is studying number theory. He has denoted a function <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>)</span> such that:</p><ul> <li> <span class="tex-span"><i>f</i>(<i>a</i>, 0) = 0</span>; </li><li> <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>) = 1 + <i>f</i>(<i>a</i>, <i>b</i> - <i>gcd</i>(<i>a</i>, <i>b</i>))</span>, where <span class="tex-span"><i>gcd</i>(<i>a</i>, <i>b</i>)</span> is the greatest common divisor of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. </li></ul><p>Vasya has two numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, and he wants to calculate <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span>. He tried to do it by himself, but found out that calculating this function the way he wants to do that might take very long time. So he decided to ask you to implement a program that will calculate this function swiftly.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span>.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span>.</p>





```input1
3 5

```




```input2
6 3

```




```output1
3

```




```output2
1

```


