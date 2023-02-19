## Description

<div><p>While Mahmoud and Ehab were practicing for IOI, they found a problem which name was Longest common subsequence. They solved it, and then Ehab challenged Mahmoud with another problem.</p><p>Given two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, find the length of their longest uncommon subsequence, which is the longest string that is a subsequence of one of them and not a subsequence of the other.</p><p>A subsequence of some string is a sequence of characters that appears in the same order in the string, The appearances don't have to be consecutive, for example, strings "<span class="tex-font-style-tt">ac</span>", "<span class="tex-font-style-tt">bc</span>", "<span class="tex-font-style-tt">abc</span>" and "<span class="tex-font-style-tt">a</span>" are subsequences of string "<span class="tex-font-style-tt">abc</span>" while strings "<span class="tex-font-style-tt">abbc</span>" and "<span class="tex-font-style-tt">acb</span>" are not. The empty string is a subsequence of any string. Any string is a subsequence of itself.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>a</i></span>, and the second line&nbsp;— string <span class="tex-span"><i>b</i></span>. Both of these strings are non-empty and consist of lowercase letters of English alphabet. The length of each string is not bigger than <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p></div><div class="output-specification"><p>If there's no uncommon subsequence, print "<span class="tex-font-style-tt">-1</span>". Otherwise print the length of the longest uncommon subsequence of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>a</i></span>, and the second line&nbsp;— string <span class="tex-span"><i>b</i></span>. Both of these strings are non-empty and consist of lowercase letters of English alphabet. The length of each string is not bigger than <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p>

## Output

<p>If there's no uncommon subsequence, print "<span class="tex-font-style-tt">-1</span>". Otherwise print the length of the longest uncommon subsequence of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p>





```input1
abcd
defgh

```




```input2
a
a

```




```output1
5

```




```output2
-1

```



## Note

<p>In the first example: you can choose "<span class="tex-font-style-tt">defgh</span>" from string <span class="tex-span"><i>b</i></span> as it is the longest subsequence of string <span class="tex-span"><i>b</i></span> that doesn't appear as a subsequence of string <span class="tex-span"><i>a</i></span>.</p>
