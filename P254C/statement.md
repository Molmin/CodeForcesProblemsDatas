## Description

<div><p>String <span class="tex-span"><i>x</i></span> is an <span class="tex-font-style-it">anagram</span> of string <span class="tex-span"><i>y</i></span>, if we can rearrange the letters in string <span class="tex-span"><i>x</i></span> and get exact string <span class="tex-span"><i>y</i></span>. For example, strings "<span class="tex-font-style-tt">DOG</span>" and "<span class="tex-font-style-tt">GOD</span>" are anagrams, so are strings "<span class="tex-font-style-tt">BABA</span>" and "<span class="tex-font-style-tt">AABB</span>", but strings "<span class="tex-font-style-tt">ABBAC</span>" and "<span class="tex-font-style-tt">CAABA</span>" are not.</p><p>You are given two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> of the same length, consisting of uppercase English letters. You need to get the anagram of string <span class="tex-span"><i>t</i></span> from string <span class="tex-span"><i>s</i></span>. You are permitted to perform the replacing operation: every operation is replacing some character from the string <span class="tex-span"><i>s</i></span> by any other character. Get the anagram of string <span class="tex-span"><i>t</i></span> in the least number of replacing operations. If you can get multiple anagrams of string <span class="tex-span"><i>t</i></span> in the least number of operations, get the lexicographically minimal one.</p><p>The lexicographic order of strings is the familiar to us "dictionary" order. Formally, the string <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span> is lexicographically smaller than string <span class="tex-span"><i>q</i></span> of the same length, if <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = <i>q</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub> = <i>q</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i> - 1</sub> = <i>q</i><sub class="lower-index"><i>k</i> - 1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub> &lt; <i>q</i><sub class="lower-index"><i>k</i></sub></span> for some <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>). Here characters in the strings are numbered from 1. The characters of the strings are compared in the alphabetic order.</p></div><div class="input-specification"><p>The input consists of two lines. The first line contains string <span class="tex-span"><i>s</i></span>, the second line contains string <span class="tex-span"><i>t</i></span>. The strings have the same length (from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span> characters) and consist of uppercase English letters.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>z</i></span> — the minimum number of replacement operations, needed to get an anagram of string <span class="tex-span"><i>t</i></span> from string <span class="tex-span"><i>s</i></span>. In the second line print the lexicographically minimum anagram that could be obtained in <span class="tex-span"><i>z</i></span> operations.</p></div>

## Input

<p>The input consists of two lines. The first line contains string <span class="tex-span"><i>s</i></span>, the second line contains string <span class="tex-span"><i>t</i></span>. The strings have the same length (from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span> characters) and consist of uppercase English letters.</p>

## Output

<p>In the first line print <span class="tex-span"><i>z</i></span> — the minimum number of replacement operations, needed to get an anagram of string <span class="tex-span"><i>t</i></span> from string <span class="tex-span"><i>s</i></span>. In the second line print the lexicographically minimum anagram that could be obtained in <span class="tex-span"><i>z</i></span> operations.</p>





```input1
ABA
CBA

```




```input2
CDBABC
ADCABD

```




```output1
1
ABC

```




```output2
2
ADBADC

```



## Note

<p>The second sample has eight anagrams of string <span class="tex-span"><i>t</i></span>, that can be obtained from string <span class="tex-span"><i>s</i></span> by replacing exactly two letters: "<span class="tex-font-style-tt">ADBADC</span>", "<span class="tex-font-style-tt">ADDABC</span>", "<span class="tex-font-style-tt">CDAABD</span>", "<span class="tex-font-style-tt">CDBAAD</span>", "<span class="tex-font-style-tt">CDBADA</span>", "<span class="tex-font-style-tt">CDDABA</span>", "<span class="tex-font-style-tt">DDAABC</span>", "<span class="tex-font-style-tt">DDBAAC</span>". These anagrams are listed in the lexicographical order. The lexicographically minimum anagram is "<span class="tex-font-style-tt">ADBADC</span>".</p>
