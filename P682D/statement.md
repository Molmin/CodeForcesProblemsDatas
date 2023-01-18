## Description

<div><p>After returned from forest, Alyona started reading a book. She noticed strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, lengths of which are <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> respectively. As usual, reading bored Alyona and she decided to pay her attention to strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, which she considered very similar.</p><p>Alyona has her favourite positive integer <span class="tex-span"><i>k</i></span> and because she is too small, <span class="tex-span"><i>k</i></span> does not exceed <span class="tex-span">10</span>. The girl wants now to choose <span class="tex-span"><i>k</i></span> disjoint non-empty substrings of string <span class="tex-span"><i>s</i></span> such that these strings appear as disjoint substrings of string <span class="tex-span"><i>t</i></span> and in the same order as they do in string <span class="tex-span"><i>s</i></span>. She is also interested in that their length is maximum possible among all variants.</p><p>Formally, Alyona wants to find a sequence of <span class="tex-span"><i>k</i></span> non-empty strings <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> satisfying following conditions:</p><ul> <li> <span class="tex-span"><i>s</i></span> can be represented as concatenation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub><i>p</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>k</i></sub><i>p</i><sub class="lower-index"><i>k</i></sub><i>a</i><sub class="lower-index"><i>k</i> + 1</sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i> + 1</sub></span> is a sequence of arbitrary strings (some of them may be possibly empty); </li><li> <span class="tex-span"><i>t</i></span> can be represented as concatenation <span class="tex-span"><i>b</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">1</sub><i>b</i><sub class="lower-index">2</sub><i>p</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>k</i></sub><i>p</i><sub class="lower-index"><i>k</i></sub><i>b</i><sub class="lower-index"><i>k</i> + 1</sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i> + 1</sub></span> is a sequence of arbitrary strings (some of them may be possibly empty); </li><li> sum of the lengths of strings in sequence is maximum possible. </li></ul><p>Please help Alyona solve this complicated problem and find at least the sum of the lengths of the strings in a desired sequence.</p><p>A <span class="tex-font-style-it">substring</span> of a string is a subsequence of consecutive characters of the string.</p></div><div class="input-specification"><p>In the first line of the input three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10</span>) are given&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>, the length of the string <span class="tex-span"><i>t</i></span> and Alyona's favourite number respectively.</p><p>The second line of the input contains string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters.</p><p>The third line of the input contains string <span class="tex-span"><i>t</i></span>, consisting of lowercase English letters.</p></div><div class="output-specification"><p>In the only line print the only non-negative integer&nbsp;— the sum of the lengths of the strings in a desired sequence.</p><p><span class="tex-font-style-bf">It is guaranteed</span>, that at least one desired sequence exists.</p></div>

## Input

<p>In the first line of the input three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10</span>) are given&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>, the length of the string <span class="tex-span"><i>t</i></span> and Alyona's favourite number respectively.</p><p>The second line of the input contains string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters.</p><p>The third line of the input contains string <span class="tex-span"><i>t</i></span>, consisting of lowercase English letters.</p>

## Output

<p>In the only line print the only non-negative integer&nbsp;— the sum of the lengths of the strings in a desired sequence.</p><p><span class="tex-font-style-bf">It is guaranteed</span>, that at least one desired sequence exists.</p>





```input1
3 2 2
abc
ab

```




```input2
9 12 4
bbaaababb
abbbabbaaaba

```




```output1
2

```




```output2
7

```



## Note

<p>The following image describes the answer for the second sample case:</p><center> <img class="tex-graphics" src="file://KuT6cRvu.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
