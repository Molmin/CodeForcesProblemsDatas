## Description

<div><p>The bear has a string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (record <span class="tex-span">|<i>s</i>|</span> is the string's length), consisting of lowercase English letters. The bear wants to count the number of such pairs of indices <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ |<i>s</i>|)</span>, that string <span class="tex-span"><i>x</i>(<i>i</i>, <i>j</i>) = <i>s</i><sub class="lower-index"><i>i</i></sub><i>s</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>j</i></sub></span> contains at least one string "<span class="tex-font-style-tt">bear</span>" as a substring.</p><p>String <span class="tex-span"><i>x</i>(<i>i</i>, <i>j</i>)</span> contains string "<span class="tex-font-style-tt">bear</span>", if there is such index <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>i</i> ≤ <i>k</i> ≤ <i>j</i> - 3)</span>, that <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub> = <i>b</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i> + 1</sub> = <i>e</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i> + 2</sub> = <i>a</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i> + 3</sub> = <i>r</i></span>.</p><p>Help the bear cope with the given problem.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 5000)</span>. It is guaranteed that the string only consists of lowercase English letters.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 5000)</span>. It is guaranteed that the string only consists of lowercase English letters.</p>

## Output

<p>Print a single number — the answer to the problem.</p>





```input1
bearbtear

```




```input2
bearaabearc

```




```output1
6

```




```output2
20

```



## Note

<p>In the first sample, the following pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> match: <span class="tex-span">(1, 4), (1, 5), (1, 6), (1, 7), (1, 8), (1, 9)</span>.</p><p>In the second sample, the following pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> match: <span class="tex-span">(1,  4), (1,  5), (1,  6), (1,  7), (1,  8), (1,  9), (1,  10), (1,  11), (2,  10), (2,  11), (3,  10), (3,  11), (4,  10), (4,  11), (5,  10), (5,  11), (6,  10), (6,  11), (7,  10), (7,  11)</span>.</p>
