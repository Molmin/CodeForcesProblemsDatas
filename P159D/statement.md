## Description

<div><p>You are given a non-empty string <span class="tex-span"><i>s</i></span> consisting of lowercase letters. Find the number of pairs of non-overlapping palindromic substrings of this string.</p><p>In a more formal way, you have to find the quantity of tuples <span class="tex-span">(<i>a</i>, <i>b</i>, <i>x</i>, <i>y</i>)</span> such that <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> &lt; <i>x</i> ≤ <i>y</i> ≤ |<i>s</i>|</span> and substrings <span class="tex-span"><i>s</i>[<i>a</i>... <i>b</i>]</span>, <span class="tex-span"><i>s</i>[<i>x</i>... <i>y</i>]</span> are palindromes.</p><p>A <span class="tex-font-style-it">palindrome</span> is a string that can be read the same way from left to right and from right to left. For example, "<span class="tex-font-style-tt">abacaba</span>", "<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">abba</span>" are palindromes.</p><p>A <span class="tex-font-style-it">substring</span> <span class="tex-span"><i>s</i>[<i>i</i>... <i>j</i>]</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ |<i>s</i>|</span>) of string <span class="tex-span"><i>s</i></span> = <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> is a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub><i>s</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>j</i></sub></span>. For example, substring <span class="tex-span"><i>s</i>[2...4]</span> of string <span class="tex-span"><i>s</i></span> = "<span class="tex-font-style-tt">abacaba</span>" equals "<span class="tex-font-style-tt">bac</span>".</p></div><div class="input-specification"><p>The first line of input contains a non-empty string <span class="tex-span"><i>s</i></span> which consists of lowercase letters ('<span class="tex-font-style-tt">a</span>'...'<span class="tex-font-style-tt">z</span>'), <span class="tex-span"><i>s</i></span> contains at most <span class="tex-span">2000</span> characters.</p></div><div class="output-specification"><p>Output a single number — the quantity of pairs of non-overlapping palindromic substrings of <span class="tex-span"><i>s</i></span>.</p><p>Please do not use the %lld format specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d format specifier.</p></div>

## Input

<p>The first line of input contains a non-empty string <span class="tex-span"><i>s</i></span> which consists of lowercase letters ('<span class="tex-font-style-tt">a</span>'...'<span class="tex-font-style-tt">z</span>'), <span class="tex-span"><i>s</i></span> contains at most <span class="tex-span">2000</span> characters.</p>

## Output

<p>Output a single number — the quantity of pairs of non-overlapping palindromic substrings of <span class="tex-span"><i>s</i></span>.</p><p>Please do not use the %lld format specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d format specifier.</p>





```input1
aa

```




```input2
aaa

```




```input3
abacaba

```




```output1
1

```




```output2
5

```




```output3
36

```


