## Description

<div><p>Palindromic characteristics of string <span class="tex-span"><i>s</i></span> with length <span class="tex-span">|<i>s</i>|</span> is a sequence of <span class="tex-span">|<i>s</i>|</span> integers, where <span class="tex-span"><i>k</i></span>-th number is the total number of non-empty substrings of <span class="tex-span"><i>s</i></span> which are <span class="tex-span"><i>k</i></span>-palindromes.</p><p>A string is <span class="tex-span">1</span>-palindrome if and only if it reads the same backward as forward.</p><p>A string is <span class="tex-span"><i>k</i></span>-palindrome (<span class="tex-span"><i>k</i> &gt; 1</span>) if and only if: </p><ol> <li> Its left half equals to its right half. </li><li> Its left and right halfs are non-empty (<span class="tex-span"><i>k</i> - 1</span>)-palindromes. </li></ol><p>The left half of string <span class="tex-span"><i>t</i></span> is its prefix of length <span class="tex-span">⌊|<i>t</i>| / 2⌋</span>, and right half&nbsp;— the suffix of the same length. <span class="tex-span">⌊|<i>t</i>| / 2⌋</span> denotes the length of string <span class="tex-span"><i>t</i></span> divided by <span class="tex-span">2</span>, rounded down.</p><p>Note that each substring is counted as many times as it appears in the string. For example, in the string "aaa" the substring "a" appears 3 times.</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>) consisting of lowercase English letters.</p></div><div class="output-specification"><p>Print <span class="tex-span">|<i>s</i>|</span> integers&nbsp;— palindromic characteristics of string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>) consisting of lowercase English letters.</p>

## Output

<p>Print <span class="tex-span">|<i>s</i>|</span> integers&nbsp;— palindromic characteristics of string <span class="tex-span"><i>s</i></span>.</p>





```input1
abba

```




```input2
abacaba

```




```output1
6 1 0 0 

```




```output2
12 4 1 0 0 0 0 

```



## Note

<p>In the first example 1-palindromes are substring «a», «b», «b», «a», «bb», «abba», the substring «bb» is 2-palindrome. There are no 3- and 4-palindromes here.</p>
