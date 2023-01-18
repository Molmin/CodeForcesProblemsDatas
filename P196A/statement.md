## Description

<div><p>You've got string <span class="tex-span"><i>s</i></span>, consisting of only lowercase English letters. Find its lexicographically maximum subsequence.</p><p>We'll call a non-empty string <span class="tex-span"><i>s</i>[<i>p</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">2</sub>... <i>p</i><sub class="lower-index"><i>k</i></sub>] = <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>k</i></sub></sub>(1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>k</i></sub> ≤ |<i>s</i>|)</span> a <span class="tex-font-style-it">subsequence</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>.</p><p>String <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index">|<i>x</i>|</sub></span> is <span class="tex-font-style-it">lexicographically larger</span> than string <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, if either <span class="tex-span">|<i>x</i>| &gt; |<i>y</i>|</span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index">|<i>y</i>|</sub> = <i>y</i><sub class="lower-index">|<i>y</i>|</sub></span>, or exists such number <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> &lt; |<i>x</i>|, <i>r</i> &lt; |<i>y</i>|)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &gt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>. Characters in lines are compared like their ASCII codes.</p></div><div class="input-specification"><p>The single line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting only of lowercase English letters. The string's length doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print the lexicographically maximum subsequence of string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The single line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting only of lowercase English letters. The string's length doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print the lexicographically maximum subsequence of string <span class="tex-span"><i>s</i></span>.</p>





```input1
ababba

```




```input2
abbcbccacbbcbaaba

```




```output1
bbba

```




```output2
cccccbba

```



## Note

<p>Let's look at samples and see what the sought subsequences look like (they are marked with uppercase bold letters).</p><p>The first sample: <span class="tex-font-style-tt">a<span class="tex-font-style-bf">B</span>a<span class="tex-font-style-bf">BBA</span></span></p><p>The second sample: <span class="tex-font-style-tt">abb<span class="tex-font-style-bf">C</span>b<span class="tex-font-style-bf">CC</span>a<span class="tex-font-style-bf">C</span>bb<span class="tex-font-style-bf">CB</span>aa<span class="tex-font-style-bf">BA</span></span></p>
