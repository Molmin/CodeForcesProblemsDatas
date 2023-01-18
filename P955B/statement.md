## Description

<div><p>Let's call a string <span class="tex-font-style-it">adorable</span> if its letters can be realigned in such a way that they form two consequent groups of equal symbols (note that different groups must contain different symbols). For example, <span class="tex-font-style-it">ababa</span> is <span class="tex-font-style-it">adorable</span> (you can transform it to <span class="tex-font-style-it">aaabb</span>, where the first three letters form a group of <span class="tex-span"><i>a</i></span>-s and others — a group of <span class="tex-span"><i>b</i></span>-s), but <span class="tex-font-style-it">cccc</span> is not since in each possible consequent partition letters in these two groups coincide.</p><p>You're given a string <span class="tex-span"><i>s</i></span>. Check whether it can be split into two non-empty subsequences such that the strings formed by these subsequences are <span class="tex-font-style-it">adorable</span>. Here a subsequence is an arbitrary set of indexes of the string.</p></div><div class="input-specification"><p>The only line contains <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup>)</span> consisting of lowercase latin letters.</p></div><div class="output-specification"><p>Print «<span class="tex-font-style-tt">Yes</span>» if the string can be split according to the criteria above or «<span class="tex-font-style-tt">No</span>» otherwise.</p><p>Each letter can be printed in arbitrary case.</p></div>

## Input

<p>The only line contains <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup>)</span> consisting of lowercase latin letters.</p>

## Output

<p>Print «<span class="tex-font-style-tt">Yes</span>» if the string can be split according to the criteria above or «<span class="tex-font-style-tt">No</span>» otherwise.</p><p>Each letter can be printed in arbitrary case.</p>





```input1
ababa

```




```input2
zzcxx

```




```input3
yeee

```




```output1
Yes

```




```output2
Yes

```




```output3
No

```



## Note

<p>In sample case two <span class="tex-font-style-it">zzcxx</span> can be split into subsequences <span class="tex-font-style-it">zc</span> and <span class="tex-font-style-it">zxx</span> each of which is <span class="tex-font-style-it">adorable</span>.</p><p>There's no suitable partition in sample case three.</p>
