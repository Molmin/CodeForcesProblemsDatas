## Description

<div><p>We'll call string <span class="tex-span"><i>s</i>[<i>a</i>, <i>b</i>] = <i>s</i><sub class="lower-index"><i>a</i></sub><i>s</i><sub class="lower-index"><i>a</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>b</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>b</i> ≤ |<i>s</i>|)</span> a <span class="tex-font-style-it">substring</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p><p>The <span class="tex-font-style-it">trace</span> of a non-empty string <span class="tex-span"><i>t</i></span> is a set of characters that the string consists of. For example, the trace of string "<span class="tex-font-style-tt">aab</span>" equals {'<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>'}.</p><p>Let's consider an arbitrary string <span class="tex-span"><i>s</i></span> and the set of its substrings with trace equal to <span class="tex-span"><i>C</i></span>. We will denote the number of substrings from this set that are maximal by inclusion by <span class="tex-span"><i>r</i>(<i>C</i>, <i>s</i>)</span>. Substring <span class="tex-span"><i>s</i>[<i>a</i>, <i>b</i>]</span> of length <span class="tex-span"><i>n</i> = <i>b</i> - <i>a</i> + 1</span> belonging to some set is called maximal by inclusion, if there is no substring <span class="tex-span"><i>s</i>[<i>x</i>, <i>y</i>]</span> in this set with length greater than <span class="tex-span"><i>n</i></span>, such that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>a</i> ≤ <i>b</i> ≤ <i>y</i> ≤ |<i>s</i>|</span>. Two substrings of string <span class="tex-span"><i>s</i></span> are considered different even if they are equal but they are located at different positions of <span class="tex-span"><i>s</i></span>.</p><p>Polycarpus got a challenging practical task on a stringology exam. He must do the following: given string <span class="tex-span"><i>s</i></span> and non-empty sets of characters <span class="tex-span"><i>C</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>C</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>C</i><sub class="lower-index"><i>m</i></sub></span>, find <span class="tex-span"><i>r</i>(<i>C</i><sub class="lower-index"><i>i</i></sub>, <i>s</i>)</span> for each set <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span>. Help Polycarpus to solve the problem as he really doesn't want to be expelled from the university and go to the army!</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>The second line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup>)</span>. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of sets <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th line contains string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> such that its trace equals <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that all characters of each string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>Note that <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily different. All given strings consist of lowercase English letters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th integer must equal <span class="tex-span"><i>r</i>(<i>C</i><sub class="lower-index"><i>i</i></sub>, <i>s</i>)</span>.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>The second line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup>)</span>. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of sets <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th line contains string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> such that its trace equals <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that all characters of each string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>Note that <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily different. All given strings consist of lowercase English letters.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th integer must equal <span class="tex-span"><i>r</i>(<i>C</i><sub class="lower-index"><i>i</i></sub>, <i>s</i>)</span>.</p>





```input1
aaaaa
2
a
a

```




```input2
abacaba
3
ac
ba
a

```




```output1
1
1

```




```output2
1
2
4

```


