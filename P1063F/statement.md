## Description

<div><p>We call a sequence of strings <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span> a <span class="tex-font-style-it">journey</span> of length <span class="tex-span"><i>k</i></span>, if for each <span class="tex-span"><i>i</i> &gt; 1</span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is a substring of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - 1</sub></span> and length of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is strictly less than length of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - 1</sub></span>. For example, <span class="tex-span">{<i>ab</i>, <i>b</i>}</span> is a journey, but <span class="tex-span">{<i>ab</i>, <i>c</i>}</span> and <span class="tex-span">{<i>a</i>, <i>a</i>}</span> are not.</p><p>Define a <span class="tex-font-style-it">journey on string</span> <span class="tex-span"><i>s</i></span> as journey <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span>, such that all its parts can be nested inside <span class="tex-span"><i>s</i></span> in such a way that there exists a sequence of strings <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, ..., <i>u</i><sub class="lower-index"><i>k</i> + 1</sub></span> (each of these strings can be empty) and <span class="tex-span"><i>s</i> = <i>u</i><sub class="lower-index">1</sub> <i>t</i><sub class="lower-index">1</sub> <i>u</i><sub class="lower-index">2</sub> <i>t</i><sub class="lower-index">2</sub>... <i>u</i><sub class="lower-index"><i>k</i></sub> <i>t</i><sub class="lower-index"><i>k</i></sub> <i>u</i><sub class="lower-index"><i>k</i> + 1</sub></span>. As an example, <span class="tex-span">{<i>ab</i>, <i>b</i>}</span> is a journey on string <span class="tex-span"><i>abb</i></span>, but not on <span class="tex-span"><i>bab</i></span> because the journey strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> should appear from the left to the right.</p><p>The <span class="tex-font-style-it">length</span> of a journey on a string is the number of strings in it. Determine the maximum possible length of a journey on the given string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> itself, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p></div><div class="output-specification"><p>Print one number&nbsp;— the maximum possible length of string journey on <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> itself, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p>

## Output

<p>Print one number&nbsp;— the maximum possible length of string journey on <span class="tex-span"><i>s</i></span>.</p>





```input1
7
abcdbcc

```




```input2
4
bbcb

```




```output1
3

```




```output2
2

```



## Note

<p>In the first sample, the string journey of maximum length is <span class="tex-span">{<i>abcd</i>, <i>bc</i>, <i>c</i>}</span>.</p><p>In the second sample, one of the suitable journeys is <span class="tex-span">{<i>bb</i>, <i>b</i>}</span>.</p>
