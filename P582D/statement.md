## Description

<div><p>For a given prime integer <span class="tex-span"><i>p</i></span> and integers <span class="tex-span">α, <i>A</i></span> calculate the number of pairs of integers <span class="tex-span">(<i>n</i>, <i>k</i>)</span>, such that <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i> ≤ <i>A</i></span> and <img align="middle" class="tex-formula" src="file://QQsmDGL0.png" style="max-width: 100.0%;max-height: 100.0%;"> is divisible by <span class="tex-span"><i>p</i><sup class="upper-index">α</sup></span>. </p><p>As the answer can be rather large, print the remainder of the answer moduly <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Let us remind you that <img align="middle" class="tex-formula" src="file://awoTfMt3.png" style="max-width: 100.0%;max-height: 100.0%;"> is the number of ways <span class="tex-span"><i>k</i></span> objects can be chosen from the set of <span class="tex-span"><i>n</i></span> objects.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>p</i></span> and <span class="tex-span">α</span> (<span class="tex-span">1 ≤ <i>p</i>, α ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>p</i></span> is prime). </p><p>The second line contains the decimal record of integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">0 ≤ <i>A</i> &lt; 10<sup class="upper-index">1000</sup></span>) without leading zeroes.</p></div><div class="output-specification"><p>In the single line print the answer to the problem.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>p</i></span> and <span class="tex-span">α</span> (<span class="tex-span">1 ≤ <i>p</i>, α ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>p</i></span> is prime). </p><p>The second line contains the decimal record of integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">0 ≤ <i>A</i> &lt; 10<sup class="upper-index">1000</sup></span>) without leading zeroes.</p>

## Output

<p>In the single line print the answer to the problem.</p>





```input1
2 2
7

```




```input2
3 1
9

```




```input3
3 3
9

```




```input4
2 4
5000

```




```output1
3

```




```output2
17

```




```output3
0

```




```output4
8576851

```



## Note

<p>In the first sample three binominal coefficients divisible by 4 are <img align="middle" class="tex-formula" src="file://ewQ83u7b.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://68zrbnxZ.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://h8rslJSI.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
