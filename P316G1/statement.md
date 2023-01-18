## Description

<div><p>Smart Beaver recently got interested in a new word game. The point is as follows: count the number of distinct good substrings of some string <span class="tex-span"><i>s</i></span>. To determine if a string is good or not the game uses rules. Overall there are <span class="tex-span"><i>n</i></span> rules. Each rule is described by a group of three <span class="tex-span">(<i>p</i>, <i>l</i>, <i>r</i>)</span>, where <span class="tex-span"><i>p</i></span> is a string and <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>l</i> ≤ <i>r</i>)</span> are integers. We’ll say that string <span class="tex-span"><i>t</i></span> complies with rule <span class="tex-span">(<i>p</i>, <i>l</i>, <i>r</i>)</span>, if the number of occurrences of string <span class="tex-span"><i>t</i></span> in string <span class="tex-span"><i>p</i></span> lies between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive. For example, string "<span class="tex-font-style-tt">ab</span>", complies with rules ("<span class="tex-font-style-tt">ab</span>", <span class="tex-span">1</span>, <span class="tex-span">2</span>) and ("<span class="tex-font-style-tt">aab</span>", <span class="tex-span">0</span>, <span class="tex-span">1</span>), but does not comply with rules ("<span class="tex-font-style-tt">cd</span>", <span class="tex-span">1</span>, <span class="tex-span">2</span>) and ("<span class="tex-font-style-tt">abab</span>", <span class="tex-span">0</span>, <span class="tex-span">1</span>).</p><p>A <span class="tex-font-style-it">substring</span> <span class="tex-span"><i>s</i>[<i>l</i>... <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|)</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (<span class="tex-span">|<i>s</i>|</span> is a length of <span class="tex-span"><i>s</i></span>) is string <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>Consider a <span class="tex-font-style-it">number of occurrences </span> of string <span class="tex-span"><i>t</i></span> in string <span class="tex-span"><i>p</i></span> as a number of pairs of integers <span class="tex-span"><i>l</i>, <i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>p</i>|)</span> such that <span class="tex-span"><i>p</i>[<i>l</i>... <i>r</i>] = <i>t</i></span>.</p><p>We’ll say that string <span class="tex-span"><i>t</i></span> is good if it complies with all <span class="tex-span"><i>n</i></span> rules. Smart Beaver asks you to help him to write a program that can calculate the number of distinct good substrings of string <span class="tex-span"><i>s</i></span>. Two substrings <span class="tex-span"><i>s</i>[<i>x</i>... <i>y</i>]</span> and <span class="tex-span"><i>s</i>[<i>z</i>... <i>w</i>]</span> are cosidered to be distinct iff <span class="tex-span"><i>s</i>[<i>x</i>... <i>y</i>] ≠ <i>s</i>[<i>z</i>... <i>w</i>]</span>.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span>. The second line contains integer <span class="tex-span"><i>n</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain the rules, one per line. Each of these lines contains a string and two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>p</i><sub class="lower-index"><i>i</i></sub>|</span>). It is guaranteed that all the given strings are non-empty and only contain lowercase English letters.</p><p>The input limits for scoring 30 points are (subproblem G1): </p><ul> <li> <span class="tex-span">0 ≤ <i>n</i> ≤ 10</span>. </li><li> The length of string <span class="tex-span"><i>s</i></span> and the maximum length of string <span class="tex-span"><i>p</i></span> is <span class="tex-span"> ≤ 200</span>. </li></ul><p>The input limits for scoring 70 points are (subproblems G1+G2): </p><ul> <li> <span class="tex-span">0 ≤ <i>n</i> ≤ 10</span>. </li><li> The length of string <span class="tex-span"><i>s</i></span> and the maximum length of string <span class="tex-span"><i>p</i></span> is <span class="tex-span"> ≤ 2000</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems G1+G2+G3): </p><ul> <li> <span class="tex-span">0 ≤ <i>n</i> ≤ 10</span>. </li><li> The length of string <span class="tex-span"><i>s</i></span> and the maximum length of string <span class="tex-span"><i>p</i></span> is <span class="tex-span"> ≤ 50000</span>. </li></ul></div><div class="output-specification"><p>Print a single integer — the number of good substrings of string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span>. The second line contains integer <span class="tex-span"><i>n</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain the rules, one per line. Each of these lines contains a string and two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>p</i><sub class="lower-index"><i>i</i></sub>|</span>). It is guaranteed that all the given strings are non-empty and only contain lowercase English letters.</p><p>The input limits for scoring 30 points are (subproblem G1): </p><ul> <li> <span class="tex-span">0 ≤ <i>n</i> ≤ 10</span>. </li><li> The length of string <span class="tex-span"><i>s</i></span> and the maximum length of string <span class="tex-span"><i>p</i></span> is <span class="tex-span"> ≤ 200</span>. </li></ul><p>The input limits for scoring 70 points are (subproblems G1+G2): </p><ul> <li> <span class="tex-span">0 ≤ <i>n</i> ≤ 10</span>. </li><li> The length of string <span class="tex-span"><i>s</i></span> and the maximum length of string <span class="tex-span"><i>p</i></span> is <span class="tex-span"> ≤ 2000</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems G1+G2+G3): </p><ul> <li> <span class="tex-span">0 ≤ <i>n</i> ≤ 10</span>. </li><li> The length of string <span class="tex-span"><i>s</i></span> and the maximum length of string <span class="tex-span"><i>p</i></span> is <span class="tex-span"> ≤ 50000</span>. </li></ul>

## Output

<p>Print a single integer — the number of good substrings of string <span class="tex-span"><i>s</i></span>.</p>





```input1
aaab
2
aa 0 0
aab 1 1

```




```input2
ltntlnen
3
n 0 0
ttlneenl 1 4
lelllt 1 1

```




```input3
a
0

```




```output1
3

```




```output2
2

```




```output3
1

```



## Note

<p>There are three good substrings in the first sample test: «<span class="tex-font-style-tt">aab</span>», «<span class="tex-font-style-tt">ab</span>» and «<span class="tex-font-style-tt">b</span>».</p><p>In the second test only substrings «<span class="tex-font-style-tt">e</span>» and «<span class="tex-font-style-tt">t</span>» are good.</p>
