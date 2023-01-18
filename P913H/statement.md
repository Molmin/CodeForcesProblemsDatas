## Description

<div><p>You generate real numbers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> as follows: </p><ul> <li> <span class="tex-span"><i>s</i><sub class="lower-index">0</sub> = 0</span>; </li><li> <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>t</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is a real number chosen independently uniformly at random between 0 and 1, inclusive. </li></ul><p>You are given real numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. You are interested in the probability that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub></span> is true for all <span class="tex-span"><i>i</i></span> simultaneously.</p><p>It can be shown that this can be represented as <img align="middle" class="tex-formula" src="file://zNPwlmrr.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime integers, and <img align="middle" class="tex-formula" src="file://tUBk6Tpf.png" style="max-width: 100.0%;max-height: 100.0%;">. Print the value of <span class="tex-span"><i>P</i>·<i>Q</i><sup class="upper-index"> - 1</sup></span> modulo <span class="tex-span">998244353</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain real numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, given with at most six digits after the decimal point (<span class="tex-span">0 &lt; <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single integer, the answer to the problem.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain real numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, given with at most six digits after the decimal point (<span class="tex-span">0 &lt; <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print a single integer, the answer to the problem.</p>





```input1
4
1.00
2
3.000000
4.0

```




```input2
1
0.50216

```




```input3
2
0.5
1.0

```




```input4
6
0.77
1.234567
2.1
1.890
2.9999
3.77

```




```output1
1

```




```output2
342677322

```




```output3
623902721

```




```output4
859831967

```



## Note

<p>In the first example, the sought probability is 1 since the sum of <span class="tex-span"><i>i</i></span> real numbers which don't exceed 1 doesn't exceed <span class="tex-span"><i>i</i></span>.</p><p>In the second example, the probability is <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> itself.</p><p>In the third example, the sought probability is <span class="tex-span">3 / 8</span>.</p>
