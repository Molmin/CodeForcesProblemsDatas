## Description

<div><p>Genos needs your help. He was asked to solve the following programming problem by Saitama:</p><p>The length of some string <span class="tex-span"><i>s</i></span> is denoted <span class="tex-span">|<i>s</i>|</span>. The Hamming distance between two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> of equal length is defined as <img align="middle" class="tex-formula" src="file://3tRTOWBL.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>t</i></span>. For example, the Hamming distance between string "<span class="tex-font-style-tt">0011</span>" and string "<span class="tex-font-style-tt">0110</span>" is <span class="tex-span">|0 - 0| + |0 - 1| + |1 - 1| + |1 - 0| = 0 + 1 + 0 + 1 = 2</span>.</p><p>Given two binary strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, find the sum of the Hamming distances between <span class="tex-span"><i>a</i></span> and all contiguous substrings of <span class="tex-span"><i>b</i></span> of length <span class="tex-span">|<i>a</i>|</span>.</p></div><div class="input-specification"><p>The first line of the input contains binary string <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ |<i>a</i>| ≤ 200 000</span>).</p><p>The second line of the input contains binary string <span class="tex-span"><i>b</i></span> (<span class="tex-span">|<i>a</i>| ≤ |<i>b</i>| ≤ 200 000</span>).</p><p>Both strings are guaranteed to consist of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the sum of Hamming distances between <span class="tex-span"><i>a</i></span> and all contiguous substrings of <span class="tex-span"><i>b</i></span> of length <span class="tex-span">|<i>a</i>|</span>.</p></div>

## Input

<p>The first line of the input contains binary string <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ |<i>a</i>| ≤ 200 000</span>).</p><p>The second line of the input contains binary string <span class="tex-span"><i>b</i></span> (<span class="tex-span">|<i>a</i>| ≤ |<i>b</i>| ≤ 200 000</span>).</p><p>Both strings are guaranteed to consist of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only.</p>

## Output

<p>Print a single integer&nbsp;— the sum of Hamming distances between <span class="tex-span"><i>a</i></span> and all contiguous substrings of <span class="tex-span"><i>b</i></span> of length <span class="tex-span">|<i>a</i>|</span>.</p>





```input1
01
00111

```




```input2
0011
0110

```




```output1
3

```




```output2
2

```



## Note

<p>For the first sample case, there are four contiguous substrings of <span class="tex-span"><i>b</i></span> of length <span class="tex-span">|<i>a</i>|</span>: "<span class="tex-font-style-tt">00</span>", "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">11</span>", and "<span class="tex-font-style-tt">11</span>". The distance between "<span class="tex-font-style-tt">01</span>" and "<span class="tex-font-style-tt">00</span>" is <span class="tex-span">|0 - 0| + |1 - 0| = 1</span>. The distance between "<span class="tex-font-style-tt">01</span>" and "<span class="tex-font-style-tt">01</span>" is <span class="tex-span">|0 - 0| + |1 - 1| = 0</span>. The distance between "<span class="tex-font-style-tt">01</span>" and "<span class="tex-font-style-tt">11</span>" is <span class="tex-span">|0 - 1| + |1 - 1| = 1</span>. Last distance counts twice, as there are two occurrences of string "<span class="tex-font-style-tt">11</span>". The sum of these edit distances is <span class="tex-span">1 + 0 + 1 + 1 = 3</span>.</p><p>The second sample case is described in the statement.</p>
