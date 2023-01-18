## Description

<div><p>You are given $n$ strings. Each string consists of lowercase English letters. Rearrange (reorder) the given strings in such a way that for every string, all strings that are placed before it are its <span class="tex-font-style-it">substrings</span>.</p><p>String $a$ is a <span class="tex-font-style-it">substring</span> of string $b$ if it is possible to choose several <span class="tex-font-style-it">consecutive</span> letters in $b$ in such a way that they form $a$. For example, string "<span class="tex-font-style-tt">for</span>" is contained as a <span class="tex-font-style-it">substring</span> in strings "<span class="tex-font-style-tt">codeforces</span>", "<span class="tex-font-style-tt">for</span>" and "<span class="tex-font-style-tt">therefore</span>", but is not contained as a <span class="tex-font-style-it">substring</span> in strings "<span class="tex-font-style-tt">four</span>", "<span class="tex-font-style-tt">fofo</span>" and "<span class="tex-font-style-tt">rof</span>".</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 100$) — the number of strings.</p><p>The next $n$ lines contain the given strings. The number of letters in each string is from $1$ to $100$, inclusive. Each string consists of lowercase English letters.</p><p>Some strings might be equal.</p></div><div class="output-specification"><p>If it is impossible to reorder $n$ given strings in required order, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) and $n$ given strings in required order.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 100$) — the number of strings.</p><p>The next $n$ lines contain the given strings. The number of letters in each string is from $1$ to $100$, inclusive. Each string consists of lowercase English letters.</p><p>Some strings might be equal.</p>

## Output

<p>If it is impossible to reorder $n$ given strings in required order, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) and $n$ given strings in required order.</p>





```input1
5
a
aba
abacaba
ba
aba

```




```input2
5
a
abacaba
ba
aba
abab

```




```input3
3
qwerty
qwerty
qwerty

```




```output1
YES
a
ba
aba
aba
abacaba

```




```output2
NO

```




```output3
YES
qwerty
qwerty
qwerty

```



## Note

<p>In the second example you cannot reorder the strings because the string "<span class="tex-font-style-tt">abab</span>" is not a <span class="tex-font-style-it">substring</span> of the string "<span class="tex-font-style-tt">abacaba</span>".</p>
