## Description

<div><p>You are given a string <span class="tex-span"><i>q</i></span>. A sequence of <span class="tex-span"><i>k</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span> is called <span class="tex-font-style-it">beautiful</span>, if the concatenation of these strings is string <span class="tex-span"><i>q</i></span> (formally, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> + <i>s</i><sub class="lower-index">2</sub> + ... + <i>s</i><sub class="lower-index"><i>k</i></sub> = <i>q</i></span>) and the first characters of these strings are distinct.</p><p>Find any <span class="tex-font-style-it">beautiful</span> sequence of strings or determine that the <span class="tex-font-style-it">beautiful</span> sequence doesn't exist.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>) — the number of strings that should be in a <span class="tex-font-style-it">beautiful</span> sequence. </p><p>The second line contains string <span class="tex-span"><i>q</i></span>, consisting of lowercase Latin letters. The length of the string is within range from <span class="tex-span">1</span> to <span class="tex-span">100</span>, inclusive.</p></div><div class="output-specification"><p>If such sequence doesn't exist, then print in a single line "NO" (without the quotes). Otherwise, print in the first line "YES" (without the quotes) and in the next <span class="tex-span"><i>k</i></span> lines print the <span class="tex-font-style-it">beautiful</span> sequence of strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>) — the number of strings that should be in a <span class="tex-font-style-it">beautiful</span> sequence. </p><p>The second line contains string <span class="tex-span"><i>q</i></span>, consisting of lowercase Latin letters. The length of the string is within range from <span class="tex-span">1</span> to <span class="tex-span">100</span>, inclusive.</p>

## Output

<p>If such sequence doesn't exist, then print in a single line "NO" (without the quotes). Otherwise, print in the first line "YES" (without the quotes) and in the next <span class="tex-span"><i>k</i></span> lines print the <span class="tex-font-style-it">beautiful</span> sequence of strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>If there are multiple possible answers, print any of them.</p>





```input1
1
abca

```




```input2
2
aaacas

```




```input3
4
abc

```




```output1
YES
abca

```




```output2
YES
aaa
cas

```




```output3
NO

```



## Note

<p>In the second sample there are two possible answers: <span class="tex-span">{"<i>aaaca</i>", "<i>s</i>"}</span> and <span class="tex-span">{"<i>aaa</i>", "<i>cas</i>"}</span>.</p>
