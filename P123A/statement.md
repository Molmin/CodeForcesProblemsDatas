## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span>, consisting of small Latin letters. Let's denote the length of the string as <span class="tex-span">|<i>s</i>|</span>. The characters in the string are numbered starting from <span class="tex-span">1</span>. </p><p>Your task is to find out if it is possible to rearrange characters in string <span class="tex-span"><i>s</i></span> so that for any prime number <span class="tex-span"><i>p</i> ≤ |<i>s</i>|</span> and for any integer <span class="tex-span"><i>i</i></span> ranging from <span class="tex-span">1</span> to <span class="tex-span">|<i>s</i>| / <i>p</i></span> (inclusive) the following condition was fulfilled <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i></sub> = <i>s</i><sub class="lower-index"><i>p</i> × <i>i</i></sub></span>. If the answer is positive, find one way to rearrange the characters.</p></div><div class="input-specification"><p>The only line contains the initial string <span class="tex-span"><i>s</i></span>, consisting of small Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>).</p></div><div class="output-specification"><p>If it is possible to rearrange the characters in the string so that the above-mentioned conditions were fulfilled, then print in the first line "<span class="tex-font-style-tt">YES</span>" (without the quotes) and print on the second line one of the possible resulting strings. If such permutation is impossible to perform, then print the single string "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The only line contains the initial string <span class="tex-span"><i>s</i></span>, consisting of small Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>).</p>

## Output

<p>If it is possible to rearrange the characters in the string so that the above-mentioned conditions were fulfilled, then print in the first line "<span class="tex-font-style-tt">YES</span>" (without the quotes) and print on the second line one of the possible resulting strings. If such permutation is impossible to perform, then print the single string "<span class="tex-font-style-tt">NO</span>".</p>





```input1
abc

```




```input2
abcd

```




```input3
xxxyxxx

```




```output1
YES
abc

```




```output2
NO

```




```output3
YES
xxxxxxy

```



## Note

<p>In the first sample any of the six possible strings will do: "abc", "acb", "bac", "bca", "cab" or "cba".</p><p>In the second sample no letter permutation will satisfy the condition at <span class="tex-span"><i>p</i> = 2</span> (<span class="tex-span"><i>s</i><sub class="lower-index">2</sub> = <i>s</i><sub class="lower-index">4</sub></span>).</p><p>In the third test any string where character "y" doesn't occupy positions 2, 3, 4, 6 will be valid.</p>
