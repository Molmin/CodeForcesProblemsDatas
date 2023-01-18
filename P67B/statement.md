## Description

<div><p>Let <span class="tex-span"><i>A</i> = {<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> be any permutation of the first <span class="tex-span"><i>n</i></span> natural numbers <span class="tex-span">{1, 2, ..., <i>n</i>}</span>. You are given a positive integer <span class="tex-span"><i>k</i></span> and another sequence <span class="tex-span"><i>B</i> = {<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub>}</span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> in <span class="tex-span"><i>A</i></span> to the left of the element <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub> = <i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> ≥ (<i>i</i> + <i>k</i>)</span>.</p><p>For example, if <span class="tex-span"><i>n</i> = 5</span>, a possible <span class="tex-span"><i>A</i></span> is <span class="tex-span">{5, 1, 4, 2, 3}</span>. For <span class="tex-span"><i>k</i> = 2</span>, <span class="tex-span"><i>B</i></span> is given by <span class="tex-span">{1, 2, 1, 0, 0}</span>. But if <span class="tex-span"><i>k</i> = 3</span>, then <span class="tex-span"><i>B</i> = {1, 1, 0, 0, 0}</span>.</p><p>For two sequences <span class="tex-span"><i>X</i> = {<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>}</span> and <span class="tex-span"><i>Y</i> = {<i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub>}</span>, let <span class="tex-span"><i>i</i></span>-th elements be the first elements such that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>, then <span class="tex-span"><i>X</i></span> is lexicographically smaller than <span class="tex-span"><i>Y</i></span>, while if <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>, then <span class="tex-span"><i>X</i></span> is lexicographically greater than <span class="tex-span"><i>Y</i></span>.</p><p>Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>B</i></span>, you need to determine the lexicographically smallest <span class="tex-span"><i>A</i></span>.</p></div><div class="input-specification"><p>The first line contains two space separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>). On the second line are <span class="tex-span"><i>n</i></span> integers specifying the values of <span class="tex-span"><i>B</i> = {<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub>}</span>.</p></div><div class="output-specification"><p>Print on a single line <span class="tex-span"><i>n</i></span> integers of <span class="tex-span"><i>A</i> = {<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> such that <span class="tex-span"><i>A</i></span> is lexicographically minimal. It is guaranteed that the solution exists.</p></div>

## Input

<p>The first line contains two space separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>). On the second line are <span class="tex-span"><i>n</i></span> integers specifying the values of <span class="tex-span"><i>B</i> = {<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub>}</span>.</p>

## Output

<p>Print on a single line <span class="tex-span"><i>n</i></span> integers of <span class="tex-span"><i>A</i> = {<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> such that <span class="tex-span"><i>A</i></span> is lexicographically minimal. It is guaranteed that the solution exists.</p>





```input1
5 2
1 2 1 0 0

```




```input2
4 2
1 0 0 0

```




```output1
4 1 5 2 3
```




```output2
2 3 1 4
```


