## Description

<div><p>Let's assume that <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are strings of positive length, called the <span class="tex-font-style-it">container</span> and the <span class="tex-font-style-it">key</span> correspondingly, string <span class="tex-span"><i>q</i></span> only consists of characters 0 and 1. Let's take a look at a simple algorithm that extracts <span class="tex-font-style-it">message</span> <span class="tex-span"><i>s</i></span> from the given container <span class="tex-span"><i>p</i></span>:</p><pre class="verbatim"><br>i = 0;<br>j = 0;<br>s = &lt;&gt;;<br>while i is less than the length of the string p<br>{<br>    if q[j] == 1, then add to the right of string s character p[i];<br>    increase variables i, j by one;<br>    if the value of the variable j equals the length of the string q, then j = 0; <br>}<br></pre><p>In the given pseudocode <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> are integer variables, <span class="tex-span"><i>s</i></span> is a string, '<span class="tex-font-style-tt">=</span>' is an assignment operator, '<span class="tex-font-style-tt">==</span>' is a comparison operation, '<span class="tex-font-style-tt">[]</span>' is the operation of obtaining the string character with the preset index, '<span class="tex-font-style-tt">&lt;&gt;</span>' is an empty string. We suppose that in all strings the characters are numbered starting from zero. </p><p>We understand that implementing such algorithm is quite easy, so your task is going to be slightly different. You need to construct the lexicographically minimum key of length <span class="tex-span"><i>k</i></span>, such that when it is used, the algorithm given above extracts message <span class="tex-span"><i>s</i></span> from container <span class="tex-span"><i>p</i></span> (otherwise find out that such key doesn't exist).</p></div><div class="input-specification"><p>The first two lines of the input are non-empty strings <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>p</i>| ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ |<i>s</i>| ≤ 200</span>), describing the container and the message, correspondingly. The strings can contain any characters with the ASCII codes from 32 to 126, inclusive.</p><p>The third line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2000)</span> — the key's length.</p></div><div class="output-specification"><p>Print the required key (string of length <span class="tex-span"><i>k</i></span>, consisting only of characters 0 and 1). If the key doesn't exist, print the single character 0.</p></div>

## Input

<p>The first two lines of the input are non-empty strings <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>p</i>| ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ |<i>s</i>| ≤ 200</span>), describing the container and the message, correspondingly. The strings can contain any characters with the ASCII codes from 32 to 126, inclusive.</p><p>The third line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2000)</span> — the key's length.</p>

## Output

<p>Print the required key (string of length <span class="tex-span"><i>k</i></span>, consisting only of characters 0 and 1). If the key doesn't exist, print the single character 0.</p>





```input1
abacaba
aba
6

```




```input2
abacaba
aba
3

```




```output1
100001

```




```output2
0

```



## Note

<p>String <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index"><i>p</i></sub></span> is <span class="tex-font-style-it">lexicographically smaller</span> than string <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index"><i>q</i></sub></span>, if either <span class="tex-span"><i>p</i> &lt; <i>q</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>p</i></sub> = <i>y</i><sub class="lower-index"><i>p</i></sub></span>, or there exists such integer <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>r</i> &lt; <i>min</i>(<i>p</i>, <i>q</i>))</span> that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &lt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>. Symbols are compared according to their ASCII codes.</p>
