## Description

<div><p>Given a string <span class="tex-span"><i>s</i></span>, determine if it contains any palindrome of length exactly <span class="tex-span">100</span> as a <span class="tex-font-style-bf">subsequence</span>. If it has any, print any one of them. If it doesn't have any, print a palindrome that is a subsequence of <span class="tex-span"><i>s</i></span> and is as long as possible.</p></div><div class="input-specification"><p>The only line of the input contains one string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>) containing only lowercase English letters.</p></div><div class="output-specification"><p>If <span class="tex-span"><i>s</i></span> contains a palindrome of length exactly <span class="tex-span">100</span> as a subsequence, print any palindrome of length <span class="tex-span">100</span> which is a subsequence of <span class="tex-span"><i>s</i></span>. If <span class="tex-span"><i>s</i></span> doesn't contain any palindromes of length exactly <span class="tex-span">100</span>, print a palindrome that is a subsequence of <span class="tex-span"><i>s</i></span> and is as long as possible.</p><p>If there exists multiple answers, you are allowed to print any of them.</p></div>

## Input

<p>The only line of the input contains one string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>) containing only lowercase English letters.</p>

## Output

<p>If <span class="tex-span"><i>s</i></span> contains a palindrome of length exactly <span class="tex-span">100</span> as a subsequence, print any palindrome of length <span class="tex-span">100</span> which is a subsequence of <span class="tex-span"><i>s</i></span>. If <span class="tex-span"><i>s</i></span> doesn't contain any palindromes of length exactly <span class="tex-span">100</span>, print a palindrome that is a subsequence of <span class="tex-span"><i>s</i></span> and is as long as possible.</p><p>If there exists multiple answers, you are allowed to print any of them.</p>





```input1
bbbabcbbb

```




```input2
rquwmzexectvnbanemsmdufrg

```




```output1
bbbcbbb

```




```output2
rumenanemur

```



## Note

<p>A subsequence of a string is a string that can be derived from it by deleting some characters without changing the order of the remaining characters. A palindrome is a string that reads the same forward or backward.</p>
