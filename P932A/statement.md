## Description

<div><p>You are given a string <span class="tex-span"><i>A</i></span>. Find a string <span class="tex-span"><i>B</i></span>, where <span class="tex-span"><i>B</i></span> is a palindrome and <span class="tex-span"><i>A</i></span> is a subsequence of <span class="tex-span"><i>B</i></span>.</p><p>A subsequence of a string is a string that can be derived from it by deleting some (not necessarily consecutive) characters without changing the order of the remaining characters. For example, "<span class="tex-font-style-tt">cotst</span>" is a subsequence of "<span class="tex-font-style-tt">contest</span>".</p><p>A palindrome is a string that reads the same forward or backward.</p><p>The length of string <span class="tex-span"><i>B</i></span> should be at most <span class="tex-span">10<sup class="upper-index">4</sup></span>. It is guaranteed that there always exists such string.</p><p>You do not need to find the shortest answer, the only restriction is that the length of string <span class="tex-span"><i>B</i></span> should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div><div class="input-specification"><p>First line contains a string <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ |<i>A</i>| ≤ 10<sup class="upper-index">3</sup></span>) consisting of lowercase Latin letters, where <span class="tex-span">|<i>A</i>|</span> is a length of <span class="tex-span"><i>A</i></span>.</p></div><div class="output-specification"><p>Output single line containing <span class="tex-span"><i>B</i></span> consisting of only lowercase Latin letters. You do not need to find the shortest answer, the only restriction is that the length of string <span class="tex-span"><i>B</i></span> should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. If there are many possible <span class="tex-span"><i>B</i></span>, print any of them.</p></div>

## Input

<p>First line contains a string <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ |<i>A</i>| ≤ 10<sup class="upper-index">3</sup></span>) consisting of lowercase Latin letters, where <span class="tex-span">|<i>A</i>|</span> is a length of <span class="tex-span"><i>A</i></span>.</p>

## Output

<p>Output single line containing <span class="tex-span"><i>B</i></span> consisting of only lowercase Latin letters. You do not need to find the shortest answer, the only restriction is that the length of string <span class="tex-span"><i>B</i></span> should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. If there are many possible <span class="tex-span"><i>B</i></span>, print any of them.</p>





```input1
aba

```




```input2
ab

```




```output1
aba
```




```output2
aabaa
```



## Note

<p>In the first example, "<span class="tex-font-style-tt">aba</span>" is a subsequence of "<span class="tex-font-style-tt">aba</span>" which is a palindrome.</p><p>In the second example, "<span class="tex-font-style-tt">ab</span>" is a subsequence of "<span class="tex-font-style-tt">aabaa</span>" which is a palindrome.</p>
