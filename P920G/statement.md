## Description

<div><p>Let's denote as <span class="tex-span"><i>L</i>(<i>x</i>, <i>p</i>)</span> an infinite sequence of integers <span class="tex-span"><i>y</i></span> such that <span class="tex-span"><i>gcd</i>(<i>p</i>, <i>y</i>) = 1</span> and <span class="tex-span"><i>y</i> &gt; <i>x</i></span> (where <span class="tex-span"><i>gcd</i></span> is the greatest common divisor of two integer numbers), sorted in ascending order. The elements of <span class="tex-span"><i>L</i>(<i>x</i>, <i>p</i>)</span> are <span class="tex-span">1</span>-indexed; for example, <span class="tex-span">9</span>, <span class="tex-span">13</span> and <span class="tex-span">15</span> are the first, the second and the third elements of <span class="tex-span"><i>L</i>(7, 22)</span>, respectively.</p><p>You have to process <span class="tex-span"><i>t</i></span> queries. Each query is denoted by three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span>, and the answer to this query is <span class="tex-span"><i>k</i></span>-th element of <span class="tex-span"><i>L</i>(<i>x</i>, <i>p</i>)</span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 30000</span>) — the number of queries to process.</p><p>Then <span class="tex-span"><i>t</i></span> lines follow. <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> for <span class="tex-span"><i>i</i></span>-th query (<span class="tex-span">1 ≤ <i>x</i>, <i>p</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> integers, where <span class="tex-span"><i>i</i></span>-th integer is the answer to <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 30000</span>) — the number of queries to process.</p><p>Then <span class="tex-span"><i>t</i></span> lines follow. <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> for <span class="tex-span"><i>i</i></span>-th query (<span class="tex-span">1 ≤ <i>x</i>, <i>p</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> integers, where <span class="tex-span"><i>i</i></span>-th integer is the answer to <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
3
7 22 1
7 22 2
7 22 3

```




```input2
5
42 42 42
43 43 43
44 44 44
45 45 45
46 46 46

```




```output1
9
13
15

```




```output2
187
87
139
128
141

```


