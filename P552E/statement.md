## Description

<div><p>Vanya is doing his maths homework. He has an expression of form <img align="middle" class="tex-formula" src="file://EaKx4J8d.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> are digits from <span class="tex-span">1</span> to <span class="tex-span">9</span>, and sign <img align="middle" class="tex-formula" src="file://TGzwCgQr.png" style="max-width: 100.0%;max-height: 100.0%;"> represents either a plus '<span class="tex-font-style-tt">+</span>' or the multiplication sign <span class="tex-font-style-tt">'*'</span>. Vanya needs to add <span class="tex-font-style-bf">one</span> pair of brackets in this expression so that to maximize the value of the resulting expression.</p></div><div class="input-specification"><p>The first line contains expression <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5001</span>, <span class="tex-span">|<i>s</i>|</span> is odd), its odd positions only contain digits from <span class="tex-span">1</span> to <span class="tex-span">9</span>, and even positions only contain signs <span class="tex-span"> + </span> and <span class="tex-span"> * </span>. </p><p>The number of signs <span class="tex-span"> * </span> doesn't exceed 15.</p></div><div class="output-specification"><p>In the first line print the maximum possible value of an expression.</p></div>

## Input

<p>The first line contains expression <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5001</span>, <span class="tex-span">|<i>s</i>|</span> is odd), its odd positions only contain digits from <span class="tex-span">1</span> to <span class="tex-span">9</span>, and even positions only contain signs <span class="tex-span"> + </span> and <span class="tex-span"> * </span>. </p><p>The number of signs <span class="tex-span"> * </span> doesn't exceed 15.</p>

## Output

<p>In the first line print the maximum possible value of an expression.</p>





```input1
3+5*7+8*4

```




```input2
2+3*5

```




```input3
3*4*5

```




```output1
303

```




```output2
25

```




```output3
60

```



## Note

<p>Note to the first sample test. <span class="tex-span">3 + 5 * (7 + 8) * 4 = 303</span>.</p><p>Note to the second sample test. <span class="tex-span">(2 + 3) * 5 = 25</span>.</p><p>Note to the third sample test. <span class="tex-span">(3 * 4) * 5 = 60</span> (also many other variants are valid, for instance, <span class="tex-span">(3) * 4 * 5 = 60</span>).</p>
