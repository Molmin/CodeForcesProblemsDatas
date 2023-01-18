## Description

<div><p>A <span class="tex-font-style-it">subsequence</span> of length <span class="tex-span">|<i>x</i>|</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>) is a string <span class="tex-span"><i>x</i> = <i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">|<i>x</i>|</sub></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index">1</sub> &lt; <i>k</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>k</i><sub class="lower-index">|<i>x</i>|</sub> ≤ |<i>s</i>|)</span>.</p><p>You've got two strings&nbsp;— <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. Let's consider all subsequences of string <span class="tex-span"><i>s</i></span>, coinciding with string <span class="tex-span"><i>t</i></span>. Is it true that each character of string <span class="tex-span"><i>s</i></span> occurs in at least one of these subsequences? In other words, is it true that for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>s</i>|)</span>, there is such subsequence <span class="tex-span"><i>x</i> = <i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">|<i>x</i>|</sub></sub></span> of string <span class="tex-span"><i>s</i></span>, that <span class="tex-span"><i>x</i> = <i>t</i></span> and for some <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>j</i> ≤ |<i>x</i>|)</span> <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub> = <i>i</i></span>.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span>, the second line contains string <span class="tex-span"><i>t</i></span>. Each line consists only of lowercase English letters. The given strings are non-empty, the length of each string does not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if each character of the string <span class="tex-span"><i>s</i></span> occurs in at least one of the described subsequences, or "<span class="tex-font-style-tt">No</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span>, the second line contains string <span class="tex-span"><i>t</i></span>. Each line consists only of lowercase English letters. The given strings are non-empty, the length of each string does not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if each character of the string <span class="tex-span"><i>s</i></span> occurs in at least one of the described subsequences, or "<span class="tex-font-style-tt">No</span>" (without the quotes) otherwise.</p>





```input1
abab
ab

```




```input2
abacaba
aba

```




```input3
abc
ba

```




```output1
Yes

```




```output2
No

```




```output3
No

```



## Note

<p>In the first sample string <span class="tex-span"><i>t</i></span> can occur in the string <span class="tex-span"><i>s</i></span> as a subsequence in three ways: <span class="tex-font-style-tt"><span class="tex-font-style-bf">ab</span>ab</span>, <span class="tex-font-style-tt"><span class="tex-font-style-bf">a</span>ba<span class="tex-font-style-bf">b</span></span> and <span class="tex-font-style-tt">ab<span class="tex-font-style-bf">ab</span></span>. In these occurrences each character of string <span class="tex-span"><i>s</i></span> occurs at least once.</p><p>In the second sample the 4-th character of the string <span class="tex-span"><i>s</i></span> doesn't occur in any occurrence of string <span class="tex-span"><i>t</i></span>.</p><p>In the third sample there is no occurrence of string <span class="tex-span"><i>t</i></span> in string <span class="tex-span"><i>s</i></span>.</p>
