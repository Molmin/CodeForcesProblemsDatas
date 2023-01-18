## Description

<div><p>You've got a string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> of length <span class="tex-span">|<i>s</i>|</span>, consisting of lowercase English letters. There also are <span class="tex-span"><i>q</i></span> queries, each query is described by two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|)</span>. The answer to the query is the number of substrings of string <span class="tex-span"><i>s</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>... <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>, which are palindromes.</p><p>String <span class="tex-span"><i>s</i>[<i>l</i>... <i>r</i>] = <i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|)</span> is a <span class="tex-font-style-it">substring</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>.</p><p>String <span class="tex-span"><i>t</i></span> is called a <span class="tex-font-style-it">palindrome</span>, if it reads the same from left to right and from right to left. Formally, if <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index">|<i>t</i>|</sub> = <i>t</i><sub class="lower-index">|<i>t</i>|</sub><i>t</i><sub class="lower-index">|<i>t</i>| - 1</sub>... <i>t</i><sub class="lower-index">1</sub></span>.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 5000)</span>. The second line contains a single integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain the queries. The <span class="tex-span"><i>i</i></span>-th of these lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|)</span> — the description of the <span class="tex-span"><i>i</i></span>-th query.</p><p>It is guaranteed that the given string consists only of lowercase English letters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers — the answers to the queries. Print the answers in the order, in which the queries are given in the input. Separate the printed numbers by whitespaces.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 5000)</span>. The second line contains a single integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain the queries. The <span class="tex-span"><i>i</i></span>-th of these lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|)</span> — the description of the <span class="tex-span"><i>i</i></span>-th query.</p><p>It is guaranteed that the given string consists only of lowercase English letters.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers — the answers to the queries. Print the answers in the order, in which the queries are given in the input. Separate the printed numbers by whitespaces.</p>





```input1
caaaba
5
1 1
1 4
2 3
4 6
4 5

```




```output1
1
7
3
4
2

```



## Note

<p>Consider the fourth query in the first test case. String <span class="tex-span"><i>s</i>[4... 6]</span> = «<span class="tex-font-style-tt">aba</span>». Its palindrome substrings are: «<span class="tex-font-style-tt">a</span>», «<span class="tex-font-style-tt">b</span>», «<span class="tex-font-style-tt">a</span>», «<span class="tex-font-style-tt">aba</span>».</p>
