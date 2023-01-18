## Description

<div><p>Piegirl got bored with binary, decimal and other integer based counting systems. Recently she discovered some interesting properties about number <img align="middle" class="tex-formula" src="file://jiAtTCmw.png" style="max-width: 100.0%;max-height: 100.0%;">, in particular that <span class="tex-span"><i>q</i><sup class="upper-index">2</sup> = <i>q</i> + 1</span>, and she thinks it would make a good base for her new unique system. She called it "golden system". In golden system the number is a non-empty string containing 0's and 1's as digits. The decimal value of expression <span class="tex-span"><i>a</i><sub class="lower-index">0</sub><i>a</i><sub class="lower-index">1</sub>...<i>a</i><sub class="lower-index"><i>n</i></sub></span> equals to <img align="middle" class="tex-formula" src="file://fgdRhKYx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Soon Piegirl found out that this system doesn't have same properties that integer base systems do and some operations can not be performed on it. She wasn't able to come up with a fast way of comparing two numbers. She is asking for your help.</p><p>Given two numbers written in golden system notation, determine which of them has larger decimal value.</p></div><div class="input-specification"><p>Input consists of two lines — one for each number. Each line contains non-empty string consisting of '0' and '1' characters. The length of each string does not exceed <span class="tex-span">100000</span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">&gt;</span>" if the first number is larger, "<span class="tex-font-style-tt">&lt;</span>" if it is smaller and "<span class="tex-font-style-tt">=</span>" if they are equal.</p></div>

## Input

<p>Input consists of two lines — one for each number. Each line contains non-empty string consisting of '0' and '1' characters. The length of each string does not exceed <span class="tex-span">100000</span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">&gt;</span>" if the first number is larger, "<span class="tex-font-style-tt">&lt;</span>" if it is smaller and "<span class="tex-font-style-tt">=</span>" if they are equal.</p>





```input1
1000
111

```




```input2
00100
11

```




```input3
110
101

```




```output1
&lt;

```




```output2
=

```




```output3
&gt;

```



## Note

<p>In the first example first number equals to <img align="middle" class="tex-formula" src="file://jAnTHbq9.png" style="max-width: 100.0%;max-height: 100.0%;">, while second number is approximately <span class="tex-span">1.618033988<sup class="upper-index">2</sup> + 1.618033988 + 1 ≈ 5.236</span>, which is clearly a bigger number.</p><p>In the second example numbers are equal. Each of them is <span class="tex-span"> ≈ 2.618</span>.</p>
