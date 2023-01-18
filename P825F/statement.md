## Description

<div><p>Ivan wants to write a letter to his friend. The letter is a string <span class="tex-span"><i>s</i></span> consisting of lowercase Latin letters.</p><p>Unfortunately, when Ivan started writing the letter, he realised that it is very long and writing the whole letter may take extremely long time. So he wants to write the <span class="tex-font-style-it">compressed version</span> of string <span class="tex-span"><i>s</i></span> instead of the string itself.</p><p>The <span class="tex-font-style-it">compressed version</span> of string <span class="tex-span"><i>s</i></span> is a sequence of strings <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub>, <i>s</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the decimal representation of number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (without any leading zeroes) and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is some string consisting of lowercase Latin letters. If Ivan writes string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> exactly <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> times, then string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> exactly <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> times, and so on, the result will be string <span class="tex-span"><i>s</i></span>.</p><p>The length of a <span class="tex-font-style-it">compressed version</span> is <span class="tex-span">|<i>c</i><sub class="lower-index">1</sub>| + |<i>s</i><sub class="lower-index">1</sub>| + |<i>c</i><sub class="lower-index">2</sub>| + |<i>s</i><sub class="lower-index">2</sub>|... |<i>c</i><sub class="lower-index"><i>k</i></sub>| + |<i>s</i><sub class="lower-index"><i>k</i></sub>|</span>. Among all <span class="tex-font-style-it">compressed versions</span> Ivan wants to choose a version such that its length is minimum possible. Help Ivan to determine minimum possible length.</p></div><div class="input-specification"><p>The only line of input contains one string <span class="tex-span"><i>s</i></span> consisting of lowercase Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 8000</span>).</p></div><div class="output-specification"><p>Output one integer number — the minimum possible length of a <span class="tex-font-style-it">compressed version</span> of <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The only line of input contains one string <span class="tex-span"><i>s</i></span> consisting of lowercase Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 8000</span>).</p>

## Output

<p>Output one integer number — the minimum possible length of a <span class="tex-font-style-it">compressed version</span> of <span class="tex-span"><i>s</i></span>.</p>





```input1
aaaaaaaaaa

```




```input2
abcab

```




```input3
cczabababab

```




```output1
3

```




```output2
6

```




```output3
7

```



## Note

<p>In the first example Ivan will choose this compressed version: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> is <span class="tex-font-style-tt">10</span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is <span class="tex-font-style-tt">a</span>.</p><p>In the second example Ivan will choose this compressed version: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> is <span class="tex-font-style-tt">1</span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is <span class="tex-font-style-tt">abcab</span>.</p><p>In the third example Ivan will choose this compressed version: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> is <span class="tex-font-style-tt">2</span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is <span class="tex-font-style-tt">c</span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> is <span class="tex-font-style-tt">1</span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> is <span class="tex-font-style-tt">z</span>, <span class="tex-span"><i>c</i><sub class="lower-index">3</sub></span> is <span class="tex-font-style-tt">4</span>, <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> is <span class="tex-font-style-tt">ab</span>.</p>
