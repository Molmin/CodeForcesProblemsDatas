## Description

<div><p>A positive integer is called a <span class="tex-font-style-it">2-3-integer</span>, if it is equal to <span class="tex-span">2<sup class="upper-index"><i>x</i></sup>·3<sup class="upper-index"><i>y</i></sup></span> for some non-negative integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. In other words, these integers are such integers that only have <span class="tex-span">2</span> and <span class="tex-span">3</span> among their prime divisors. For example, integers <span class="tex-span">1</span>, <span class="tex-span">6</span>, <span class="tex-span">9</span>, <span class="tex-span">16</span> and <span class="tex-span">108</span> — are 2-3 integers, while <span class="tex-span">5</span>, <span class="tex-span">10</span>, <span class="tex-span">21</span> and <span class="tex-span">120</span> are not.</p><p>Print the number of <span class="tex-font-style-it">2-3-integers</span> on the given segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, i.&nbsp;e. the number of sich <span class="tex-font-style-it">2-3-integers</span> <span class="tex-span"><i>t</i></span> that <span class="tex-span"><i>l</i> ≤ <i>t</i> ≤ <i>r</i></span>.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single integer the number of <span class="tex-font-style-it">2-3-integers</span> on the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single integer the number of <span class="tex-font-style-it">2-3-integers</span> on the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>.</p>





```input1
1 10

```




```input2
100 200

```




```input3
1 2000000000

```




```output1
7

```




```output2
5

```




```output3
326

```



## Note

<p>In the first example the <span class="tex-font-style-it">2-3-integers</span> are <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">6</span>, <span class="tex-span">8</span> and <span class="tex-span">9</span>.</p><p>In the second example the <span class="tex-font-style-it">2-3-integers</span> are <span class="tex-span">108</span>, <span class="tex-span">128</span>, <span class="tex-span">144</span>, <span class="tex-span">162</span> and <span class="tex-span">192</span>.</p>
