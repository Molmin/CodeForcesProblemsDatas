## Description

<div><p>DZY loves collecting special strings which only contain lowercase letters. For each lowercase letter <span class="tex-span"><i>c</i></span> DZY knows its value <span class="tex-span"><i>w</i><sub class="lower-index"><i>c</i></sub></span>. For each special string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (<span class="tex-span">|<i>s</i>|</span> is the length of the string) he represents its value with a function <span class="tex-span"><i>f</i>(<i>s</i>)</span>, where </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://FoHbMcu6.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Now DZY has a string <span class="tex-span"><i>s</i></span>. He wants to insert <span class="tex-span"><i>k</i></span> lowercase letters into this string in order to get the largest possible value of the resulting string. Can you help him calculate the largest possible value he could get? </p></div><div class="input-specification"><p>The first line contains a single string <span class="tex-span"><i>s</i>&nbsp;(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">3</sup>)</span>.</p><p>The second line contains a single integer <span class="tex-span"><i>k</i>&nbsp;(0 ≤ <i>k</i> ≤ 10<sup class="upper-index">3</sup>)</span>.</p><p>The third line contains twenty-six integers from <span class="tex-span"><i>w</i><sub class="lower-index"><i>a</i></sub></span> to <span class="tex-span"><i>w</i><sub class="lower-index"><i>z</i></sub></span>. Each such number is non-negative and doesn't exceed <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>Print a single integer — the largest possible value of the resulting string DZY could get.</p></div>

## Input

<p>The first line contains a single string <span class="tex-span"><i>s</i>&nbsp;(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">3</sup>)</span>.</p><p>The second line contains a single integer <span class="tex-span"><i>k</i>&nbsp;(0 ≤ <i>k</i> ≤ 10<sup class="upper-index">3</sup>)</span>.</p><p>The third line contains twenty-six integers from <span class="tex-span"><i>w</i><sub class="lower-index"><i>a</i></sub></span> to <span class="tex-span"><i>w</i><sub class="lower-index"><i>z</i></sub></span>. Each such number is non-negative and doesn't exceed <span class="tex-span">1000</span>.</p>

## Output

<p>Print a single integer — the largest possible value of the resulting string DZY could get.</p>





```input1
abc
3
1 2 2 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1

```




```output1
41

```



## Note

<p>In the test sample DZY can obtain "<span class="tex-font-style-tt">abcbbc</span>", <span class="tex-span"><i>value</i> = 1·1 + 2·2 + 3·2 + 4·2 + 5·2 + 6·2 = 41</span>.</p>
