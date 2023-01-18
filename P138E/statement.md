## Description

<div><p>Katya recently started to invent programming tasks and prepare her own contests. What she does not like is boring and simple constraints. Katya is fed up with all those "<span class="tex-span"><i>N</i></span> does not exceed a thousand" and "the sum of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> does not exceed a million" and she decided to come up with something a little more complicated.</p><p>The last problem written by Katya deals with strings. The input is a string of small Latin letters. To make the statement longer and strike terror into the people who will solve the contest, Katya came up with the following set of <span class="tex-span"><i>k</i></span> restrictions of the same type (characters in restrictions can be repeated and some restrictions may contradict each other): </p><ul> <li> The number of characters <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> in a string is not less than <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> and not more than <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>. </li><li> ... </li><li> The number of characters <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in a string is not less than <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and not more than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> ... </li><li> The number of characters <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span> in a string is not less than <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and not more than <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>. </li></ul><p>However, having decided that it is too simple and obvious, Katya added the following condition: a string meets no less than <span class="tex-span"><i>L</i></span> and not more than <span class="tex-span"><i>R</i></span> constraints from the above given list.</p><p>Katya does not like to compose difficult and mean tests, so she just took a big string <span class="tex-span"><i>s</i></span> and wants to add to the tests all its substrings that meet the constraints. However, Katya got lost in her conditions and asked you to count the number of substrings of the string <span class="tex-span"><i>s</i></span> that meet the conditions (each occurrence of the substring is counted separately).</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of small Latin letters. The length of the string <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>The second line contains three space-separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> (<span class="tex-span">0 ≤ <i>L</i> ≤ <i>R</i> ≤ <i>k</i> ≤ 500</span>).</p><p>Next <span class="tex-span"><i>k</i></span> lines contain Katya's constrictions in the following form "<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>". All letters <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are small Latin letters, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> are integers (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>). Letters <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily different.</p></div><div class="output-specification"><p>Print a single number — the number of substrings that meet the constrictions.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of small Latin letters. The length of the string <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>The second line contains three space-separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> (<span class="tex-span">0 ≤ <i>L</i> ≤ <i>R</i> ≤ <i>k</i> ≤ 500</span>).</p><p>Next <span class="tex-span"><i>k</i></span> lines contain Katya's constrictions in the following form "<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>". All letters <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are small Latin letters, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> are integers (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>). Letters <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily different.</p>

## Output

<p>Print a single number — the number of substrings that meet the constrictions.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
codeforces
2 0 0
o 1 2
e 1 2

```




```input2
codeforces
2 1 1
o 1 2
o 1 2

```




```output1
7

```




```output2
0

```



## Note

<p>In the first test we should count the number of strings that do not contain characters "<span class="tex-font-style-tt">e</span>" and "<span class="tex-font-style-tt">o</span>". All such strings are as follows (in the order of occurrence in the initial string from the left to the right): "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">d</span>"', "<span class="tex-font-style-tt">f</span>", "<span class="tex-font-style-tt">r</span>", "<span class="tex-font-style-tt">rc</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">s</span>".</p><p>In the second test we cannot achieve fulfilling exactly one of the two identical constrictions, so the answer is 0.</p>
