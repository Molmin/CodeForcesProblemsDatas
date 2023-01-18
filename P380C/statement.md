## Description

<div><p>Sereja has a bracket sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>, or, in other words, a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>Sereja needs to answer <span class="tex-span"><i>m</i></span> queries, each of them is described by two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. The answer to the <span class="tex-span"><i>i</i></span>-th query is the length of the maximum correct bracket subsequence of sequence <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>, <i>s</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub>, ..., <i>s</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span>. Help Sereja answer all queries.</p><p>You can find the definitions for a subsequence and a correct bracket sequence in the notes.</p></div><div class="input-specification"><p>The first line contains a sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> without any spaces. Each character is either a "<span class="tex-font-style-tt">(</span>" or a "<span class="tex-font-style-tt">)</span>". The second line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Print the answer to each question on a single line. Print the answers in the order they go in the input.</p></div>

## Input

<p>The first line contains a sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> without any spaces. Each character is either a "<span class="tex-font-style-tt">(</span>" or a "<span class="tex-font-style-tt">)</span>". The second line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Print the answer to each question on a single line. Print the answers in the order they go in the input.</p>





```input1
())(())(())(
7
1 1
2 3
1 2
1 12
8 12
5 11
2 10

```




```output1
0
0
2
10
4
6
6

```



## Note

<p>A <span class="tex-font-style-it">subsequence</span> of length <span class="tex-span">|<i>x</i>|</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>) is string <span class="tex-span"><i>x</i> = <i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>k</i><sub class="lower-index">|<i>x</i>|</sub></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index">1</sub> &lt; <i>k</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>k</i><sub class="lower-index">|<i>x</i>|</sub> ≤ |<i>s</i>|)</span>.</p><p>A <span class="tex-font-style-it">correct bracket sequence</span> is a bracket sequence that can be transformed into a correct aryphmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the characters of the string. For example, bracket sequences "<span class="tex-font-style-tt">()()</span>", "<span class="tex-font-style-tt">(())</span>" are correct (the resulting expressions "<span class="tex-font-style-tt">(1)+(1)</span>", "<span class="tex-font-style-tt">((1+1)+1)</span>"), and "<span class="tex-font-style-tt">)(</span>" and "<span class="tex-font-style-tt">(</span>" are not.</p><p>For the third query required sequence will be «<span class="tex-font-style-tt">()</span>».</p><p>For the fourth query required sequence will be «<span class="tex-font-style-tt">()(())(())</span>».</p>
