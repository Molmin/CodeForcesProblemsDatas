## Description

<div><p>In mathematics, a <span class="tex-font-style-it">subsequence</span> is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements. For example, the sequence <span class="tex-font-style-tt">BDF</span> is a subsequence of <span class="tex-font-style-tt">ABCDEF</span>. A <span class="tex-font-style-it">substring</span> of a string is a continuous subsequence of the string. For example, <span class="tex-font-style-tt">BCD</span> is a substring of <span class="tex-font-style-tt">ABCDEF</span>.</p><p>You are given two strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and another string called <span class="tex-span"><i>virus</i></span>. Your task is to find the longest common subsequence of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, such that it doesn't contain <span class="tex-span"><i>virus</i></span> as a substring.</p></div><div class="input-specification"><p>The input contains three strings in three separate lines: <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>virus</i></span> (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>|, |<i>virus</i>| ≤ 100</span>). Each string consists only of uppercase English letters.</p></div><div class="output-specification"><p>Output the longest common subsequence of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> without <span class="tex-span"><i>virus</i></span> as a substring. If there are multiple answers, any of them will be accepted. </p><p>If there is no valid common subsequence, output 0.</p></div>

## Input

<p>The input contains three strings in three separate lines: <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>virus</i></span> (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>|, |<i>virus</i>| ≤ 100</span>). Each string consists only of uppercase English letters.</p>

## Output

<p>Output the longest common subsequence of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> without <span class="tex-span"><i>virus</i></span> as a substring. If there are multiple answers, any of them will be accepted. </p><p>If there is no valid common subsequence, output 0.</p>





```input1
AJKEQSLOBSROFGZ
OVGURWZLWVLUXTH
OZ

```




```input2
AA
A
A

```




```output1
ORZ

```




```output2
0

```


