## Description

<div><p>One day Polycarpus got hold of two non-empty strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, consisting of lowercase Latin letters. Polycarpus is quite good with strings, so he immediately wondered, how many different pairs of "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" are there, such that <span class="tex-span"><i>x</i></span> is a substring of string <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>y</i></span> is a subsequence of string <span class="tex-span"><i>t</i></span>, and the content of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> is the same. Two pairs are considered different, if they contain different substrings of string <span class="tex-span"><i>s</i></span> or different subsequences of string <span class="tex-span"><i>t</i></span>. Read the whole statement to understand the definition of different substrings and subsequences.</p><p>The <span class="tex-font-style-it">length</span> of string <span class="tex-span"><i>s</i></span> is the number of characters in it. If we denote the length of the string <span class="tex-span"><i>s</i></span> as <span class="tex-span">|<i>s</i>|</span>, we can write the string as <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>.</p><p>A <span class="tex-font-style-it">substring</span> of <span class="tex-span"><i>s</i></span> is a non-empty string <span class="tex-span"><i>x</i> = <i>s</i>[<i>a</i>... <i>b</i>] = <i>s</i><sub class="lower-index"><i>a</i></sub><i>s</i><sub class="lower-index"><i>a</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ |<i>s</i>|</span>). For example, "<span class="tex-font-style-tt">code</span>" and "<span class="tex-font-style-tt">force</span>" are substrings or "<span class="tex-font-style-tt">codeforces</span>", while "<span class="tex-font-style-tt">coders</span>" is not. Two substrings <span class="tex-span"><i>s</i>[<i>a</i>... <i>b</i>]</span> and <span class="tex-span"><i>s</i>[<i>c</i>... <i>d</i>]</span> are considered to be <span class="tex-font-style-it">different</span> if <span class="tex-span"><i>a</i> ≠ <i>c</i></span> or <span class="tex-span"><i>b</i> ≠ <i>d</i></span>. For example, if <span class="tex-span"><i>s</i></span>="<span class="tex-font-style-tt">codeforces</span>", <span class="tex-span"><i>s</i>[2...2]</span> and <span class="tex-span"><i>s</i>[6...6]</span> are different, though their content is the same.</p><p>A <span class="tex-font-style-it">subsequence</span> of <span class="tex-span"><i>s</i></span> is a non-empty string <span class="tex-span"><i>y</i> = <i>s</i>[<i>p</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">2</sub>... <i>p</i><sub class="lower-index">|<i>y</i>|</sub>] = <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">|<i>y</i>|</sub></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index">|<i>y</i>|</sub> ≤ |<i>s</i>|</span>). For example, "<span class="tex-font-style-tt">coders</span>" is a subsequence of "<span class="tex-font-style-tt">codeforces</span>". Two subsequences <span class="tex-span"><i>u</i> = <i>s</i>[<i>p</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">2</sub>... <i>p</i><sub class="lower-index">|<i>u</i>|</sub>]</span> and <span class="tex-span"><i>v</i> = <i>s</i>[<i>q</i><sub class="lower-index">1</sub><i>q</i><sub class="lower-index">2</sub>... <i>q</i><sub class="lower-index">|<i>v</i>|</sub>]</span> are considered <span class="tex-font-style-it">different</span> if the sequences <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are different.</p></div><div class="input-specification"><p>The input consists of two lines. The first of them contains <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>), and the second one contains <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 5000</span>). Both strings consist of lowercase Latin letters.</p></div><div class="output-specification"><p>Print a single number — the number of different pairs "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" such that <span class="tex-span"><i>x</i></span> is a substring of string <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>y</i></span> is a subsequence of string <span class="tex-span"><i>t</i></span>, and the content of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> is the same. As the answer can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The input consists of two lines. The first of them contains <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>), and the second one contains <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 5000</span>). Both strings consist of lowercase Latin letters.</p>

## Output

<p>Print a single number — the number of different pairs "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" such that <span class="tex-span"><i>x</i></span> is a substring of string <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>y</i></span> is a subsequence of string <span class="tex-span"><i>t</i></span>, and the content of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> is the same. As the answer can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
aa
aa

```




```input2
codeforces
forceofcode

```




```output1
5

```




```output2
60

```



## Note

<p>Let's write down all pairs "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" that form the answer in the first sample: "<span class="tex-span"><i>s</i>[1...1]</span> <span class="tex-span"><i>t</i>[1]</span>", "<span class="tex-span"><i>s</i>[2...2]</span> <span class="tex-span"><i>t</i>[1]</span>", "<span class="tex-span"><i>s</i>[1...1]</span> <span class="tex-span"><i>t</i>[2]</span>","<span class="tex-span"><i>s</i>[2...2]</span> <span class="tex-span"><i>t</i>[2]</span>", "<span class="tex-span"><i>s</i>[1...2]</span> <span class="tex-span"><i>t</i>[1&nbsp;2]</span>".</p>
