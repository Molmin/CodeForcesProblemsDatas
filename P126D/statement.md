## Description

<div><p>Fibonacci numbers have the following form:</p><center class="tex-equation"><span class="tex-span"><i>F</i><sub class="lower-index">1</sub> = 1, </span></center> <center class="tex-equation"><span class="tex-span"><i>F</i><sub class="lower-index">2</sub> = 2, </span></center> <center class="tex-equation"><span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub> = <i>F</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>F</i><sub class="lower-index"><i>i</i> - 2</sub>, <i>i</i> &gt; 2.</span></center><p>Let's consider some non-empty set <span class="tex-span"><i>S</i> = {<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub>}</span>, consisting of <span class="tex-font-style-bf">different</span> Fibonacci numbers. Let's find the sum of values of this set's elements:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://7QuLvQEH.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Let's call the set <span class="tex-span"><i>S</i></span> a number <span class="tex-span"><i>n</i></span>'s <span class="tex-font-style-it">decomposition into Fibonacci sum</span>. </p><p>It's easy to see that several numbers have several decompositions into Fibonacci sum. For example, for <span class="tex-span">13</span> we have <span class="tex-span">13, 5 + 8, 2 + 3 + 8</span> — three decompositions, and for <span class="tex-span">16</span>: <span class="tex-span">3 + 13, 1 + 2 + 13, 3 + 5 + 8, 1 + 2 + 5 + 8</span> — four decompositions.</p><p>By the given number <span class="tex-span"><i>n</i></span> determine the number of its possible different decompositions into Fibonacci sum.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>t</i></span> — the number of tests (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the following <span class="tex-span"><i>t</i></span> lines contains one test.</p><p>Each test is an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div><div class="output-specification"><p>For each input data test print a single number on a single line — the answer to the problem.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>t</i></span> — the number of tests (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the following <span class="tex-span"><i>t</i></span> lines contains one test.</p><p>Each test is an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>

## Output

<p>For each input data test print a single number on a single line — the answer to the problem.</p>





```input1
2
13
16

```




```output1
3
4

```



## Note

<p>Two decompositions are different if there exists a number that is contained in the first decomposition, but is not contained in the second one. Decompositions that differ only in the order of summands are considered equal.</p>
