## Description

<div><p>A string is called palindrome if it reads the same from left to right and from right to left. For example "<span class="tex-font-style-tt">kazak</span>", "<span class="tex-font-style-tt">oo</span>", "<span class="tex-font-style-tt">r</span>" and "<span class="tex-font-style-tt">mikhailrubinchikkihcniburliahkim</span>" are palindroms, but strings "<span class="tex-font-style-tt">abb</span>" and "<span class="tex-font-style-tt">ij</span>" are not.</p><p>You are given string <span class="tex-span"><i>s</i></span> consisting of lowercase Latin letters. At once you can choose any position in the string and change letter in that position to any other lowercase letter. So after each changing the length of the string doesn't change. At first you can change some letters in <span class="tex-span"><i>s</i></span>. Then you can permute the order of letters as you want. Permutation doesn't count as changes. </p><p>You should obtain palindrome with the minimal number of changes. If there are several ways to do that you should get the lexicographically (alphabetically) smallest palindrome. So firstly you should minimize the number of changes and then minimize the palindrome lexicographically.</p></div><div class="input-specification"><p>The only line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>) consisting of only lowercase Latin letters.</p></div><div class="output-specification"><p>Print the lexicographically smallest palindrome that can be obtained with the minimal number of changes.</p></div>

## Input

<p>The only line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>) consisting of only lowercase Latin letters.</p>

## Output

<p>Print the lexicographically smallest palindrome that can be obtained with the minimal number of changes.</p>





```input1
aabc

```




```input2
aabcd

```




```output1
abba

```




```output2
abcba

```


