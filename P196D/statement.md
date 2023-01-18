## Description

<div><p>In problems on strings one often has to find a string with some particular properties. The problem authors were reluctant to waste time on thinking of a name for some string so they called it <span class="tex-font-style-it">good</span>. A string is good if it doesn't have palindrome substrings longer than or equal to <span class="tex-span"><i>d</i></span>. </p><p>You are given string <span class="tex-span"><i>s</i></span>, consisting only of lowercase English letters. Find a good string <span class="tex-span"><i>t</i></span> with length <span class="tex-span">|<i>s</i>|</span>, consisting of lowercase English letters, which is lexicographically larger than <span class="tex-span"><i>s</i></span>. Of all such strings string <span class="tex-span"><i>t</i></span> must be lexicographically minimum.</p><p>We will call a non-empty string <span class="tex-span"><i>s</i>[<i>a</i>&nbsp;...&nbsp;<i>b</i>] = <i>s</i><sub class="lower-index"><i>a</i></sub><i>s</i><sub class="lower-index"><i>a</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>b</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>b</i> ≤ |<i>s</i>|)</span> a <span class="tex-font-style-it">substring</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>.</p><p>A non-empty string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> is called <span class="tex-font-style-it">a palindrome</span> if for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> the following fulfills: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>n</i> - <i>i</i> + 1</sub></span>. In other words, palindrome read the same in both directions.</p><p>String <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index">|<i>x</i>|</sub></span> is <span class="tex-font-style-it">lexicographically larger</span> than string <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, if either <span class="tex-span">|<i>x</i>| &gt; |<i>y</i>|</span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index">|<i>y</i>|</sub> = <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, or there exists such number <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> &lt; |<i>x</i>|, <i>r</i> &lt; |<i>y</i>|)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &gt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>. Characters in such strings are compared like their ASCII codes.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ |<i>s</i>|</span>).</p><p>The second line contains a non-empty string <span class="tex-span"><i>s</i></span>, its length is no more than <span class="tex-span">4·10<sup class="upper-index">5</sup></span> characters. The string consists of lowercase English letters.</p></div><div class="output-specification"><p>Print the good string that lexicographically follows <span class="tex-span"><i>s</i></span>, has the same length and consists of only lowercase English letters. If such string does not exist, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ |<i>s</i>|</span>).</p><p>The second line contains a non-empty string <span class="tex-span"><i>s</i></span>, its length is no more than <span class="tex-span">4·10<sup class="upper-index">5</sup></span> characters. The string consists of lowercase English letters.</p>

## Output

<p>Print the good string that lexicographically follows <span class="tex-span"><i>s</i></span>, has the same length and consists of only lowercase English letters. If such string does not exist, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p>





```input1
3
aaaaaaa

```




```input2
3
zzyzzzz

```




```input3
4
abbabbbabbb

```




```output1
aabbcaa

```




```output2
Impossible

```




```output3
abbbcaaabab

```


