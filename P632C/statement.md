## Description

<div><p>You're given a list of <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You'd like to concatenate them together in some order such that the resulting string would be lexicographically smallest.</p><p>Given the list of strings, output the lexicographically smallest concatenation.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of strings (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains one string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 50</span>) consisting of only lowercase English letters. The sum of string lengths will not exceed <span class="tex-span">5·10<sup class="upper-index">4</sup></span>.</p></div><div class="output-specification"><p>Print the only string <span class="tex-span"><i>a</i></span> — the lexicographically smallest string concatenation.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of strings (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains one string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 50</span>) consisting of only lowercase English letters. The sum of string lengths will not exceed <span class="tex-span">5·10<sup class="upper-index">4</sup></span>.</p>

## Output

<p>Print the only string <span class="tex-span"><i>a</i></span> — the lexicographically smallest string concatenation.</p>





```input1
4
abba
abacaba
bcd
er

```




```input2
5
x
xx
xxa
xxaa
xxaaa

```




```input3
3
c
cb
cba

```




```output1
abacabaabbabcder

```




```output2
xxaaaxxaaxxaxxx

```




```output3
cbacbc

```


