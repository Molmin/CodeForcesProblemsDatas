## Description

<div><p>Let's introduce the designation <img align="middle" class="tex-formula" src="file://MonXRE2B.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>x</i></span> is a string, <span class="tex-span"><i>n</i></span> is a positive integer and operation "<span class="tex-span"> + </span>" is the string concatenation operation. For example, <span class="tex-span">[<i>abc</i>, 2] = <i>abcabc</i></span>.</p><p>We'll say that string <span class="tex-span"><i>s</i></span> <span class="tex-font-style-it">can be obtained</span> from string <span class="tex-span"><i>t</i></span>, if we can remove some characters from string <span class="tex-span"><i>t</i></span> and obtain string <span class="tex-span"><i>s</i></span>. For example, strings <span class="tex-span"><i>ab</i></span> and <span class="tex-span"><i>aсba</i></span> can be obtained from string <span class="tex-span"><i>xacbac</i></span>, and strings <span class="tex-span"><i>bx</i></span> and <span class="tex-span"><i>aaa</i></span> cannot be obtained from it.</p><p>Sereja has two strings, <span class="tex-span"><i>w</i> = [<i>a</i>, <i>b</i>]</span> and <span class="tex-span"><i>q</i> = [<i>c</i>, <i>d</i>]</span>. He wants to find such maximum integer <span class="tex-span"><i>p</i></span> <span class="tex-span">(<i>p</i> &gt; 0)</span>, that <span class="tex-span">[<i>q</i>, <i>p</i>]</span> can be obtained from string <span class="tex-span"><i>w</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>b</i>, <i>d</i> ≤ 10<sup class="upper-index">7</sup>)</span>. The second line contains string <span class="tex-span"><i>a</i></span>. The third line contains string <span class="tex-span"><i>c</i></span>. The given strings are not empty and consist of lowercase English letters. Their lengths do not exceed <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>In a single line print an integer — the largest number <span class="tex-span"><i>p</i></span>. If the required value of <span class="tex-span"><i>p</i></span> doesn't exist, print 0.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>b</i>, <i>d</i> ≤ 10<sup class="upper-index">7</sup>)</span>. The second line contains string <span class="tex-span"><i>a</i></span>. The third line contains string <span class="tex-span"><i>c</i></span>. The given strings are not empty and consist of lowercase English letters. Their lengths do not exceed <span class="tex-span">100</span>.</p>

## Output

<p>In a single line print an integer — the largest number <span class="tex-span"><i>p</i></span>. If the required value of <span class="tex-span"><i>p</i></span> doesn't exist, print 0.</p>





```input1
10 3
abab
bab

```




```output1
3

```


