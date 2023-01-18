## Description

<div><p><span class="tex-span"><i>N</i></span> variables <span class="tex-span"><i>X</i><sub class="lower-index">1</sub>, ..., <i>X</i><sub class="lower-index"><i>N</i></sub></span> can have positive integer values. You are given <span class="tex-span"><i>K</i></span> constraints for these value that look like "the values of variables <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>X</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>X</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>M</i></sub></sub></span> are different". Among all possible lists of values of these variables that satisfy these constraints select the ones which have minimum possible <span class="tex-span"><i>max</i>(<i>X</i><sub class="lower-index"><i>i</i></sub>)</span>. Output lexicographically least of these lists.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>K</i> ≤ 100</span>) — the number of variables and the number of constraints.</p><p>The following <span class="tex-span"><i>K</i></span> lines contain the constraints, formatted as follows: the first number in the line <span class="tex-span"><i>M</i></span> (<span class="tex-span">2 ≤ <i>M</i> ≤ <i>N</i></span>) gives the number of variables in the constraint. After it follow <span class="tex-span"><i>M</i></span> space-separated integers <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, ..., <i>i</i><sub class="lower-index"><i>M</i></sub></span> — the indices of the variables used in the constraint (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>j</i></sub> ≤ <i>N</i></span>). All <span class="tex-span"><i>i</i><sub class="lower-index"><i>j</i></sub></span> in one constraint are different.</p></div><div class="output-specification"><p>Output the values of <span class="tex-span"><i>X</i><sub class="lower-index">1</sub>, <i>X</i><sub class="lower-index">2</sub>, ..., <i>X</i><sub class="lower-index"><i>N</i></sub></span> in a single line, separated with single spaces.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>K</i> ≤ 100</span>) — the number of variables and the number of constraints.</p><p>The following <span class="tex-span"><i>K</i></span> lines contain the constraints, formatted as follows: the first number in the line <span class="tex-span"><i>M</i></span> (<span class="tex-span">2 ≤ <i>M</i> ≤ <i>N</i></span>) gives the number of variables in the constraint. After it follow <span class="tex-span"><i>M</i></span> space-separated integers <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, ..., <i>i</i><sub class="lower-index"><i>M</i></sub></span> — the indices of the variables used in the constraint (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>j</i></sub> ≤ <i>N</i></span>). All <span class="tex-span"><i>i</i><sub class="lower-index"><i>j</i></sub></span> in one constraint are different.</p>

## Output

<p>Output the values of <span class="tex-span"><i>X</i><sub class="lower-index">1</sub>, <i>X</i><sub class="lower-index">2</sub>, ..., <i>X</i><sub class="lower-index"><i>N</i></sub></span> in a single line, separated with single spaces.</p>





```input1
2 1
2 1 2

```




```input2
3 2
2 1 2
2 2 3

```




```output1
1 2

```




```output2
1 2 1

```


