## Description

<div><p>The new ITone 6 has been released recently and George got really keen to buy it. Unfortunately, he didn't have enough money, so George was going to work as a programmer. Now he faced the following problem at the work.</p><p>Given a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. You are to choose <span class="tex-span"><i>k</i></span> pairs of integers:</p><p> </p><center class="tex-equation"><span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>], [<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>], ..., [<i>l</i><sub class="lower-index"><i>k</i></sub>, <i>r</i><sub class="lower-index"><i>k</i></sub>]&nbsp;(1 ≤ <i>l</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">1</sub> &lt; <i>l</i><sub class="lower-index">2</sub> ≤ <i>r</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>;&nbsp;<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub> + 1 = <i>m</i>), </span></center><p>in such a way that the value of sum <img align="middle" class="tex-formula" src="file://4rRjccFh.png" style="max-width: 100.0%;max-height: 100.0%;"> is maximal possible. Help George to cope with the task.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ (<i>m</i> × <i>k</i>) ≤ <i>n</i> ≤ 5000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print an integer in a single line — the maximum possible value of sum.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ (<i>m</i> × <i>k</i>) ≤ <i>n</i> ≤ 5000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print an integer in a single line — the maximum possible value of sum.</p>





```input1
5 2 1
1 2 3 4 5

```




```input2
7 1 3
2 10 7 18 5 33 0

```




```output1
9

```




```output2
61

```


