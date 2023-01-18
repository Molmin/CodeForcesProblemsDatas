## Description

<div><p><span class="tex-font-style-underline">This problem's actual name, "Lexicographically Largest Palindromic Subsequence" is too long to fit into the page headline.</span></p><p>You are given string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters only. Find its lexicographically largest palindromic subsequence.</p><p>We'll call a non-empty string <span class="tex-span"><i>s</i>[<i>p</i><sub class="lower-index">1</sub></span><span class="tex-span"><i>p</i><sub class="lower-index">2</sub>... <i>p</i><sub class="lower-index"><i>k</i></sub>]</span> = <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>k</i></sub></sub></span> (<span class="tex-span">1</span> <span class="tex-span"> ≤ </span> <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span"> ≤ </span> <span class="tex-span">|<i>s</i>|</span>) a <span class="tex-font-style-underline">subsequence</span> of string <span class="tex-span"><i>s</i></span> = <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span><span class="tex-span"><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>. For example, strings "<span class="tex-font-style-tt">abcb</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">abacaba</span>" are subsequences of string "<span class="tex-font-style-tt">abacaba</span>".</p><p>String <span class="tex-span"><i>x</i></span> = <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span><span class="tex-span"><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index">|<i>x</i>|</sub></span> is <span class="tex-font-style-underline">lexicographically larger</span> than string <span class="tex-span"><i>y</i></span> = <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span><span class="tex-span"><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span> if either <span class="tex-span">|<i>x</i>|</span> &gt; <span class="tex-span">|<i>y</i>|</span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index">|<i>y</i>|</sub> = <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, or there exists such number <span class="tex-span"><i>r</i></span> (<span class="tex-span"><i>r</i> &lt; |<i>x</i>|</span>, <span class="tex-span"><i>r</i> &lt; |<i>y</i>|</span>) that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i>  +  1</sub> &gt; <i>y</i><sub class="lower-index"><i>r</i>  +  1</sub></span>. Characters in the strings are compared according to their ASCII codes. For example, string "<span class="tex-font-style-tt">ranger</span>" is lexicographically larger than string "<span class="tex-font-style-tt">racecar</span>" and string "<span class="tex-font-style-tt">poster</span>" is lexicographically larger than string "<span class="tex-font-style-tt">post</span>".</p><p>String <span class="tex-span"><i>s</i></span> = <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span><span class="tex-span"><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> is a <span class="tex-font-style-underline">palindrome</span> if it matches string <span class="tex-span"><i>rev</i>(<i>s</i>)</span> = <span class="tex-span"><i>s</i><sub class="lower-index">|<i>s</i>|</sub></span><span class="tex-span"><i>s</i><sub class="lower-index">|<i>s</i>| - 1</sub>... <i>s</i><sub class="lower-index">1</sub></span>. In other words, a string is a palindrome if it reads the same way from left to right and from right to left. For example, palindromic strings are "<span class="tex-font-style-tt">racecar</span>", "<span class="tex-font-style-tt">refer</span>" and "<span class="tex-font-style-tt">z</span>".</p></div><div class="input-specification"><p>The only input line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters only. Its length does not exceed <span class="tex-span">10</span>.</p></div><div class="output-specification"><p>Print the lexicographically largest palindromic subsequence of string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The only input line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters only. Its length does not exceed <span class="tex-span">10</span>.</p>

## Output

<p>Print the lexicographically largest palindromic subsequence of string <span class="tex-span"><i>s</i></span>.</p>





```input1
radar

```




```input2
bowwowwow

```




```input3
codeforces

```




```input4
mississipp

```




```output1
rr

```




```output2
wwwww

```




```output3
s

```




```output4
ssss

```



## Note

<p>Among all distinct subsequences of string "<span class="tex-font-style-tt">radar</span>" the following ones are palindromes: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">d</span>", "<span class="tex-font-style-tt">r</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">rr</span>", "<span class="tex-font-style-tt">ada</span>", "<span class="tex-font-style-tt">rar</span>", "<span class="tex-font-style-tt">rdr</span>", "<span class="tex-font-style-tt">raar</span>" and "<span class="tex-font-style-tt">radar</span>". The lexicographically largest of them is "<span class="tex-font-style-tt">rr</span>".</p>
