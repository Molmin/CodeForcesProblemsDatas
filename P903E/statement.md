## Description

<div><p>We had a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters. We made <span class="tex-span"><i>k</i></span> copies of this string, thus obtaining <span class="tex-span"><i>k</i></span> identical strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>. After that, in each of these strings we swapped exactly two characters (the characters we swapped could be identical, but they had different indices in the string).</p><p>You are given <span class="tex-span"><i>k</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>, and you have to restore any string <span class="tex-span"><i>s</i></span> so that it is possible to obtain these strings by performing aforementioned operations. Note that the total length of the strings you are given doesn't exceed 5000 (that is, <span class="tex-span"><i>k</i>·<i>n</i> ≤ 5000</span>).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2500, 2 ≤ <i>n</i> ≤ 5000, <i>k</i>&nbsp;·&nbsp;<i>n</i> ≤ 5000</span>) — the number of strings we obtained, and the length of each of these strings.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>, each consisting of exactly <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-bf">any</span> suitable string <span class="tex-span"><i>s</i></span>, or <span class="tex-font-style-tt">-1</span> if such string doesn't exist.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2500, 2 ≤ <i>n</i> ≤ 5000, <i>k</i>&nbsp;·&nbsp;<i>n</i> ≤ 5000</span>) — the number of strings we obtained, and the length of each of these strings.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>, each consisting of exactly <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p>

## Output

<p>Print <span class="tex-font-style-bf">any</span> suitable string <span class="tex-span"><i>s</i></span>, or <span class="tex-font-style-tt">-1</span> if such string doesn't exist.</p>





```input1
3 4
abac
caab
acba

```




```input2
3 4
kbbu
kbub
ubkb

```




```input3
5 4
abcd
dcba
acbd
dbca
zzzz

```




```output1
acab

```




```output2
kbub

```




```output3
-1

```



## Note

<p>In the first example <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is obtained by swapping the second and the fourth character in <span class="tex-font-style-tt">acab</span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> is obtained by swapping the first and the second character, and to get <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span>, we swap the third and the fourth character.</p><p>In the second example <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is obtained by swapping the third and the fourth character in <span class="tex-font-style-tt">kbub</span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> — by swapping the second and the fourth, and <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> — by swapping the first and the third.</p><p>In the third example it's impossible to obtain given strings by aforementioned operations.</p>
