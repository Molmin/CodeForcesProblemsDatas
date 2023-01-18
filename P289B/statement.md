## Description

<div><p>Little penguin Polo has an <span class="tex-span"><i>n</i> × <i>m</i></span> matrix, consisting of integers. Let's index the matrix rows from 1 to <span class="tex-span"><i>n</i></span> from top to bottom and let's index the columns from 1 to <span class="tex-span"><i>m</i></span> from left to right. Let's represent the matrix element on the intersection of row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span> as <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>.</p><p>In one move the penguin can add or subtract number <span class="tex-span"><i>d</i></span> from some matrix element. Find the minimum number of moves needed to make all matrix elements equal. If the described plan is impossible to carry out, say so.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100, 1 ≤ <i>d</i> ≤ 10<sup class="upper-index">4</sup>)</span> — the matrix sizes and the <span class="tex-span"><i>d</i></span> parameter. Next <span class="tex-span"><i>n</i></span> lines contain the matrix: the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th row is the matrix element <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>.</p></div><div class="output-specification"><p>In a single line print a single integer — the minimum number of moves the penguin needs to make all matrix elements equal. If that is impossible, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100, 1 ≤ <i>d</i> ≤ 10<sup class="upper-index">4</sup>)</span> — the matrix sizes and the <span class="tex-span"><i>d</i></span> parameter. Next <span class="tex-span"><i>n</i></span> lines contain the matrix: the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th row is the matrix element <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>.</p>

## Output

<p>In a single line print a single integer — the minimum number of moves the penguin needs to make all matrix elements equal. If that is impossible, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p>





```input1
2 2 2
2 4
6 8

```




```input2
1 2 7
6 7

```




```output1
4

```




```output2
-1

```


