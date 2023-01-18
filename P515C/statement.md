## Description

<div><p>Drazil is playing a math game with Varda.</p><p>Let's define <img align="middle" class="tex-formula" src="file://1Q73tayK.png" style="max-width: 100.0%;max-height: 100.0%;"> for positive integer <span class="tex-span"><i>x</i></span> as a product of factorials of its digits. For example, <img align="middle" class="tex-formula" src="file://JB4u0XYu.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>First, they choose a decimal number <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> digits that contains at least one digit larger than <span class="tex-span">1</span>. This number may possibly start with leading zeroes. Then they should find maximum positive number <span class="tex-span"><i>x</i></span> satisfying following two conditions:</p><p>1. <span class="tex-span"><i>x</i></span> doesn't contain neither digit <span class="tex-span">0</span> nor digit <span class="tex-span">1</span>.</p><p>2. <img align="middle" class="tex-formula" src="file://HeSselCK.png" style="max-width: 100.0%;max-height: 100.0%;"> = <img align="middle" class="tex-formula" src="file://iWNvE0PL.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Help friends find such number.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15</span>) — the number of digits in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits of <span class="tex-span"><i>a</i></span>. There is at least one digit in <span class="tex-span"><i>a</i></span> that is larger than <span class="tex-span">1</span>. Number <span class="tex-span"><i>a</i></span> may possibly contain leading zeroes.</p></div><div class="output-specification"><p>Output a maximum possible integer satisfying the conditions above. There should be no zeroes and ones in this number decimal representation.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15</span>) — the number of digits in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits of <span class="tex-span"><i>a</i></span>. There is at least one digit in <span class="tex-span"><i>a</i></span> that is larger than <span class="tex-span">1</span>. Number <span class="tex-span"><i>a</i></span> may possibly contain leading zeroes.</p>

## Output

<p>Output a maximum possible integer satisfying the conditions above. There should be no zeroes and ones in this number decimal representation.</p>





```input1
4
1234

```




```input2
3
555

```




```output1
33222

```




```output2
555

```



## Note

<p>In the first case, <img align="middle" class="tex-formula" src="file://FeQak38j.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
