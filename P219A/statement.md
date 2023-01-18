## Description

<div><p>A string is called a <span class="tex-span"><i>k</i></span>-string if it can be represented as <span class="tex-span"><i>k</i></span> concatenated copies of some string. For example, the string "<span class="tex-font-style-tt">aabaabaabaab</span>" is at the same time a 1-string, a 2-string and a 4-string, but it is not a 3-string, a 5-string, or a 6-string and so on. Obviously any string is a 1-string.</p><p>You are given a string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters and a positive integer <span class="tex-span"><i>k</i></span>. Your task is to reorder the letters in the string <span class="tex-span"><i>s</i></span> in such a way that the resulting string is a <span class="tex-span"><i>k</i></span>-string.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>). The second line contains <span class="tex-span"><i>s</i></span>, all characters in <span class="tex-span"><i>s</i></span> are lowercase English letters. The string length <span class="tex-span"><i>s</i></span> satisfies the inequality <span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>Rearrange the letters in string <span class="tex-span"><i>s</i></span> in such a way that the result is a <span class="tex-span"><i>k</i></span>-string. Print the result on a single output line. If there are multiple solutions, print any of them.</p><p>If the solution doesn't exist, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>). The second line contains <span class="tex-span"><i>s</i></span>, all characters in <span class="tex-span"><i>s</i></span> are lowercase English letters. The string length <span class="tex-span"><i>s</i></span> satisfies the inequality <span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>Rearrange the letters in string <span class="tex-span"><i>s</i></span> in such a way that the result is a <span class="tex-span"><i>k</i></span>-string. Print the result on a single output line. If there are multiple solutions, print any of them.</p><p>If the solution doesn't exist, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p>





```input1
2
aazz

```




```input2
3
abcabcabz

```




```output1
azaz

```




```output2
-1

```


