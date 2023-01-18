## Description

<div><p>You are given a non-empty string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. You have to pick <span class="tex-font-style-bf">exactly one non-empty substring</span> of <span class="tex-span"><i>s</i></span> and shift all its letters '<span class="tex-font-style-tt">z</span>' <img align="middle" class="tex-formula" src="file://ptPyKAXg.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">y</span>' <img align="middle" class="tex-formula" src="file://nqzHqs83.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">x</span>' <img align="middle" class="tex-formula" src="file://BjVBSvnR.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">b</span>' <img align="middle" class="tex-formula" src="file://vsM4cYZK.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">a</span>' <img align="middle" class="tex-formula" src="file://Hotjggky.png" style="max-width: 100.0%;max-height: 100.0%;"> '<span class="tex-font-style-tt">z</span>'. In other words, each character is replaced with the previous character of English alphabet and '<span class="tex-font-style-tt">a</span>' is replaced with '<span class="tex-font-style-tt">z</span>'.</p><p>What is the lexicographically minimum string that can be obtained from <span class="tex-span"><i>s</i></span> by performing this shift exactly once?</p></div><div class="input-specification"><p>The only line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>) consisting of lowercase English letters.</p></div><div class="output-specification"><p>Print the lexicographically minimum string that can be obtained from <span class="tex-span"><i>s</i></span> by shifting letters of exactly one non-empty substring.</p></div>

## Input

<p>The only line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>) consisting of lowercase English letters.</p>

## Output

<p>Print the lexicographically minimum string that can be obtained from <span class="tex-span"><i>s</i></span> by shifting letters of exactly one non-empty substring.</p>





```input1
codeforces

```




```input2
abacaba

```




```output1
bncdenqbdr

```




```output2
aaacaba

```



## Note

<p>String <span class="tex-span"><i>s</i></span> is lexicographically smaller than some other string <span class="tex-span"><i>t</i></span> of the same length if there exists some <span class="tex-span">1 ≤ <i>i</i> ≤ |<i>s</i>|</span>, such that <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> = <i>t</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub> = <i>t</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>t</i><sub class="lower-index"><i>i</i> - 1</sub></span>, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p>
