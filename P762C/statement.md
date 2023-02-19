## Description

<div><p>You are given two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. You have to remove the minimum possible number of <span class="tex-font-style-bf">consecutive</span> (standing one after another) characters from string <span class="tex-span"><i>b</i></span> in such a way that it becomes a subsequence of string <span class="tex-span"><i>a</i></span>. It can happen that you will not need to remove any characters at all, or maybe you will have to remove all of the characters from <span class="tex-span"><i>b</i></span> and make it empty.</p><p>Subsequence of string <span class="tex-span"><i>s</i></span> is any such string that can be obtained by erasing zero or more characters (<span class="tex-font-style-bf">not necessarily consecutive</span>) from string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>a</i></span>, and the second line&nbsp;— string <span class="tex-span"><i>b</i></span>. Both of these strings are nonempty and consist of lowercase letters of English alphabet. The length of each string is no bigger than <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p></div><div class="output-specification"><p>On the first line output a subsequence of string <span class="tex-span"><i>a</i></span>, obtained from <span class="tex-span"><i>b</i></span> by erasing the minimum number of consecutive characters.</p><p>If the answer consists of zero characters, output «<span class="tex-font-style-tt">-</span>» (a minus sign).</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>a</i></span>, and the second line&nbsp;— string <span class="tex-span"><i>b</i></span>. Both of these strings are nonempty and consist of lowercase letters of English alphabet. The length of each string is no bigger than <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p>

## Output

<p>On the first line output a subsequence of string <span class="tex-span"><i>a</i></span>, obtained from <span class="tex-span"><i>b</i></span> by erasing the minimum number of consecutive characters.</p><p>If the answer consists of zero characters, output «<span class="tex-font-style-tt">-</span>» (a minus sign).</p>





```input1
hi
bob

```




```input2
abca
accepted

```




```input3
abacaba
abcdcba

```




```output1
-

```




```output2
ac

```




```output3
abcba

```



## Note

<p>In the first example strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> don't share any symbols, so the longest string that you can get is empty.</p><p>In the second example <span class="tex-font-style-tt">ac</span> is a subsequence of <span class="tex-span"><i>a</i></span>, and at the same time you can obtain it by erasing consecutive symbols <span class="tex-font-style-tt">cepted</span> from string <span class="tex-span"><i>b</i></span>.</p>
