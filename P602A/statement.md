## Description

<div><p>After seeing the "ALL YOUR BASE ARE BELONG TO US" meme for the first time, numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> realised that they have different bases, which complicated their relations.</p><p>You're given a number <span class="tex-span"><i>X</i></span> represented in base <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span> and a number <span class="tex-span"><i>Y</i></span> represented in base <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>. Compare those two numbers.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">2 ≤ <i>b</i><sub class="lower-index"><i>x</i></sub> ≤ 40</span>), where <span class="tex-span"><i>n</i></span> is the number of digits in the <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span>-based representation of <span class="tex-span"><i>X</i></span>. </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>x</i></sub></span>) — the digits of <span class="tex-span"><i>X</i></span>. They are given in the order from the most significant digit to the least significant one.</p><p>The following two lines describe <span class="tex-span"><i>Y</i></span> in the same way: the third line contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>, <span class="tex-span">2 ≤ <i>b</i><sub class="lower-index"><i>y</i></sub> ≤ 40</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub> ≠ <i>b</i><sub class="lower-index"><i>y</i></sub></span>), where <span class="tex-span"><i>m</i></span> is the number of digits in the <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>-based representation of <span class="tex-span"><i>Y</i></span>, and the fourth line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>y</i></sub></span>) — the digits of <span class="tex-span"><i>Y</i></span>.</p><p>There will be no leading zeroes. Both <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> will be positive. All digits of both numbers are given in the standard decimal numeral system.</p></div><div class="output-specification"><p>Output a single character (quotes for clarity): </p><ul> <li> '<span class="tex-font-style-tt">&lt;</span>' if <span class="tex-span"><i>X</i> &lt; <i>Y</i></span> </li><li> '<span class="tex-font-style-tt">&gt;</span>' if <span class="tex-span"><i>X</i> &gt; <i>Y</i></span> </li><li> '<span class="tex-font-style-tt">=</span>' if <span class="tex-span"><i>X</i> = <i>Y</i></span> </li></ul></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">2 ≤ <i>b</i><sub class="lower-index"><i>x</i></sub> ≤ 40</span>), where <span class="tex-span"><i>n</i></span> is the number of digits in the <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span>-based representation of <span class="tex-span"><i>X</i></span>. </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>x</i></sub></span>) — the digits of <span class="tex-span"><i>X</i></span>. They are given in the order from the most significant digit to the least significant one.</p><p>The following two lines describe <span class="tex-span"><i>Y</i></span> in the same way: the third line contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>, <span class="tex-span">2 ≤ <i>b</i><sub class="lower-index"><i>y</i></sub> ≤ 40</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub> ≠ <i>b</i><sub class="lower-index"><i>y</i></sub></span>), where <span class="tex-span"><i>m</i></span> is the number of digits in the <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>-based representation of <span class="tex-span"><i>Y</i></span>, and the fourth line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>y</i></sub></span>) — the digits of <span class="tex-span"><i>Y</i></span>.</p><p>There will be no leading zeroes. Both <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> will be positive. All digits of both numbers are given in the standard decimal numeral system.</p>

## Output

<p>Output a single character (quotes for clarity): </p><ul> <li> '<span class="tex-font-style-tt">&lt;</span>' if <span class="tex-span"><i>X</i> &lt; <i>Y</i></span> </li><li> '<span class="tex-font-style-tt">&gt;</span>' if <span class="tex-span"><i>X</i> &gt; <i>Y</i></span> </li><li> '<span class="tex-font-style-tt">=</span>' if <span class="tex-span"><i>X</i> = <i>Y</i></span> </li></ul>





```input1
6 2
1 0 1 1 1 1
2 10
4 7

```




```input2
3 3
1 0 2
2 5
2 4

```




```input3
7 16
15 15 4 0 0 7 10
7 9
4 8 0 3 1 5 0

```




```output1
=

```




```output2
&lt;

```




```output3
&gt;

```



## Note

<p>In the first sample, <span class="tex-span"><i>X</i> = 101111<sub class="lower-index">2</sub> = 47<sub class="lower-index">10</sub> = <i>Y</i></span>.</p><p>In the second sample, <span class="tex-span"><i>X</i> = 102<sub class="lower-index">3</sub> = 21<sub class="lower-index">5</sub></span> and <span class="tex-span"><i>Y</i> = 24<sub class="lower-index">5</sub> = 112<sub class="lower-index">3</sub></span>, thus <span class="tex-span"><i>X</i> &lt; <i>Y</i></span>.</p><p>In the third sample, <img align="middle" class="tex-formula" src="file://ff9F7wlw.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>Y</i> = 4803150<sub class="lower-index">9</sub></span>. We may notice that <span class="tex-span"><i>X</i></span> starts with much larger digits and <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span> is much larger than <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>, so <span class="tex-span"><i>X</i></span> is clearly larger than <span class="tex-span"><i>Y</i></span>.</p>
