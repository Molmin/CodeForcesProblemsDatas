## Description

<div><p>There are less than 60 years left till the 900-th birthday anniversary of a famous Italian mathematician Leonardo Fibonacci. Of course, such important anniversary needs much preparations.</p><p>Dima is sure that it'll be great to learn to solve the following problem by the Big Day: You're given a set <span class="tex-span"><i>A</i></span>, consisting of numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>l</i> + 1</span>, <span class="tex-span"><i>l</i> + 2</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>r</i></span>; let's consider all its <span class="tex-span"><i>k</i></span>-element subsets; for each such subset let's find the largest common divisor of Fibonacci numbers with indexes, determined by the subset elements. Among all found common divisors, Dima is interested in the largest one.</p><p>Dima asked to remind you that Fibonacci numbers are elements of a numeric sequence, where <span class="tex-span"><i>F</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>F</i><sub class="lower-index">2</sub> = 1</span>, <span class="tex-span"><i>F</i><sub class="lower-index"><i>n</i></sub> = <i>F</i><sub class="lower-index"><i>n</i> - 1</sub> + <i>F</i><sub class="lower-index"><i>n</i> - 2</sub></span> for <span class="tex-span"><i>n</i> ≥ 3</span>.</p><p>Dima has more than half a century ahead to solve the given task, but you only have two hours. Count the residue from dividing the sought largest common divisor by <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>l</i> &lt; <i>r</i> ≤ 10<sup class="upper-index">12</sup>;&nbsp;2 ≤ <i>k</i> ≤ <i>r</i> - <i>l</i> + 1)</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer — the residue from dividing the sought greatest common divisor by <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>l</i> &lt; <i>r</i> ≤ 10<sup class="upper-index">12</sup>;&nbsp;2 ≤ <i>k</i> ≤ <i>r</i> - <i>l</i> + 1)</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer — the residue from dividing the sought greatest common divisor by <span class="tex-span"><i>m</i></span>.</p>





```input1
10 1 8 2

```




```input2
10 1 8 3

```




```output1
3

```




```output2
1

```


