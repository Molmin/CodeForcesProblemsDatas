## Description

<div><p>A <span class="tex-font-style-it">substring</span> of a string is a contiguous subsequence of that string. So, string <span class="tex-font-style-tt">bca</span> is substring of string <span class="tex-font-style-tt">abcabc</span>, but string <span class="tex-font-style-tt">cc</span> is not.</p><p>A <span class="tex-font-style-it">repeating block</span> is a string formed by concatenating some string with itself. So, string <span class="tex-font-style-tt">abcabc</span> is a repeating block, but strings <span class="tex-font-style-tt">abcabd</span>, <span class="tex-font-style-tt">ababab</span> are not.</p><p>You've got a sequence of Latin characters (string). At each step you find the shortest substring that is a repeating block, if there exists more than one you must choose the leftmost. As the substring is of form <span class="tex-span"><i>XX</i></span> (<span class="tex-span"><i>X</i></span> — some string) you replace this substring with <span class="tex-span"><i>X</i></span>, in other words you delete one of the <span class="tex-span"><i>X</i></span> substrings in the substring. You repeat this process until there remains no repeating block in the string. </p><p>How would the final string looks like? Look at the sample explanation to understand the statement more precise.</p></div><div class="input-specification"><p>In the first line of input you're given a string of small Latin characters with length between <span class="tex-span">1</span> to <span class="tex-span">50000</span>, inclusive.</p></div><div class="output-specification"><p>Print the final string after applying changes.</p></div>

## Input

<p>In the first line of input you're given a string of small Latin characters with length between <span class="tex-span">1</span> to <span class="tex-span">50000</span>, inclusive.</p>

## Output

<p>Print the final string after applying changes.</p>





```input1
abccabc

```




```input2
aaaabaaab

```




```input3
birdbirdbirdistheword

```




```output1
abc

```




```output2
ab

```




```output3
birdistheword

```



## Note

<p>At the first sample the string transforms as follows: <span class="tex-font-style-tt">abccabc</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">abcabc</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">abc</span>.</p><p>At the second sample the string transforms as follows: <span class="tex-font-style-tt">aaaabaaab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">aaabaaab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">aabaaab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">abaaab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">abaab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">abab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">ab</span>.</p>
