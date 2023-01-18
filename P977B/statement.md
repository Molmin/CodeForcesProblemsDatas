## Description

<div><p>Two-gram is an ordered pair (i.e. string of length two) of capital Latin letters. For example, "<span class="tex-font-style-tt">AZ</span>", "<span class="tex-font-style-tt">AA</span>", "<span class="tex-font-style-tt">ZA</span>" — three distinct two-grams.</p><p>You are given a string $s$ consisting of $n$ capital Latin letters. Your task is to find <span class="tex-font-style-bf">any</span> two-gram contained in the given string <span class="tex-font-style-bf">as a substring</span> (i.e. two consecutive characters of the string) maximal number of times. For example, for string $s$ = "<span class="tex-font-style-tt">BBAABBBA</span>" the answer is two-gram "<span class="tex-font-style-tt">BB</span>", which contained in $s$ three times. In other words, find any most frequent two-gram.</p><p>Note that occurrences of the two-gram can overlap with each other.</p></div><div class="input-specification"><p>The first line of the input contains integer number $n$ ($2 \le n \le 100$) — the length of string $s$. The second line of the input contains the string $s$ consisting of $n$ capital Latin letters.</p></div><div class="output-specification"><p>Print the only line containing exactly two capital Latin letters — <span class="tex-font-style-bf">any</span> two-gram contained in the given string $s$ <span class="tex-font-style-bf">as a substring</span> (i.e. two consecutive characters of the string) maximal number of times.</p></div>

## Input

<p>The first line of the input contains integer number $n$ ($2 \le n \le 100$) — the length of string $s$. The second line of the input contains the string $s$ consisting of $n$ capital Latin letters.</p>

## Output

<p>Print the only line containing exactly two capital Latin letters — <span class="tex-font-style-bf">any</span> two-gram contained in the given string $s$ <span class="tex-font-style-bf">as a substring</span> (i.e. two consecutive characters of the string) maximal number of times.</p>





```input1
7
ABACABA

```




```input2
5
ZZZAA

```




```output1
AB

```




```output2
ZZ

```



## Note

<p>In the first example "<span class="tex-font-style-tt">BA</span>" is also valid answer.</p><p>In the second example the only two-gram "<span class="tex-font-style-tt">ZZ</span>" can be printed because it contained in the string "<span class="tex-font-style-tt">ZZZAA</span>" two times.</p>
