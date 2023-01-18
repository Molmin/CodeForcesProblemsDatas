## Description

<div><p>Levko loves strings of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters, very much. He has one such string <span class="tex-span"><i>s</i></span>. For each string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>n</i></span>, Levko defines its beauty relative to <span class="tex-span"><i>s</i></span> as the number of pairs of indexes <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i>)</span>, such that substring <span class="tex-font-style-bf"><span class="tex-span"><i>t</i>[<i>i</i>..<i>j</i>]</span> is lexicographically larger than substring <span class="tex-span"><i>s</i>[<i>i</i>..<i>j</i>]</span></span>.</p><p>The boy wondered how many strings <span class="tex-span"><i>t</i></span> are there, such that their beauty relative to <span class="tex-span"><i>s</i></span> equals exactly <span class="tex-span"><i>k</i></span>. Help him, find the remainder after division this number by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>A substring <span class="tex-span"><i>s</i>[<i>i</i>..<i>j</i>]</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> is string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub><i>s</i><sub class="lower-index"><i>i</i>  +  1</sub>... <i>s</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>String <span class="tex-span"><i>x</i>  =  <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index"><i>p</i></sub></span> is lexicographically larger than string <span class="tex-span"><i>y</i>  =  <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index"><i>p</i></sub></span>, if there is such number <span class="tex-span"><i>r</i></span> (<span class="tex-span"><i>r</i> &lt; <i>p</i></span>), that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>  =  <i>y</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">2</sub>  =  <i>y</i><sub class="lower-index">2</sub>,  ... ,  <i>x</i><sub class="lower-index"><i>r</i></sub>  =  <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i>  +  1</sub> &gt; <i>y</i><sub class="lower-index"><i>r</i>  +  1</sub></span>. The string characters are compared by their ASCII codes.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 2000</span>).</p><p>The second line contains a non-empty string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. String <span class="tex-span"><i>s</i></span> consists only of lowercase English letters. </p></div><div class="output-specification"><p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 2000</span>).</p><p>The second line contains a non-empty string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. String <span class="tex-span"><i>s</i></span> consists only of lowercase English letters. </p>

## Output

<p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 2
yz

```




```input2
2 3
yx

```




```input3
4 7
abcd

```




```output1
26

```




```output2
2

```




```output3
21962

```


