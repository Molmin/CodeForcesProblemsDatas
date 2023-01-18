## Description

<div><p>Little penguin Polo adores strings. But most of all he adores strings of length <span class="tex-span"><i>n</i></span>.</p><p>One day he wanted to find a string that meets the following conditions:</p><ol> <li> The string consists of <span class="tex-span"><i>n</i></span> lowercase English letters (that is, the string's length equals <span class="tex-span"><i>n</i></span>), exactly <span class="tex-span"><i>k</i></span> of these letters are distinct. </li><li> No two neighbouring letters of a string coincide; that is, if we represent a string as <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span>, then the following inequality holds, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>s</i><sub class="lower-index"><i>i</i> + 1</sub>(1 ≤ <i>i</i> &lt; <i>n</i>)</span>. </li><li> Among all strings that meet points 1 and 2, the required string is lexicographically smallest. </li></ol><p>Help him find such string or state that such string doesn't exist.</p><p>String <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index"><i>p</i></sub></span> is <span class="tex-font-style-it">lexicographically less</span> than string <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index"><i>q</i></sub></span>, if either <span class="tex-span"><i>p</i> &lt; <i>q</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>p</i></sub> = <i>y</i><sub class="lower-index"><i>p</i></sub></span>, or there is such number <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> &lt; <i>p</i>, <i>r</i> &lt; <i>q</i>)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &lt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>. The characters of the strings are compared by their ASCII codes.</p></div><div class="input-specification"><p>A single line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>k</i> ≤ 26)</span> — the string's length and the number of distinct letters.</p></div><div class="output-specification"><p>In a single line print the required string. If there isn't such string, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div>

## Input

<p>A single line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>k</i> ≤ 26)</span> — the string's length and the number of distinct letters.</p>

## Output

<p>In a single line print the required string. If there isn't such string, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p>





```input1
7 4

```




```input2
4 7

```




```output1
ababacd

```




```output2
-1

```


