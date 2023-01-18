## Description

<div><p>Professor GukiZ was playing with arrays again and accidentally discovered new function, which he called <span class="tex-span"><i>GukiZiana</i></span>. For given array <span class="tex-span"><i>a</i></span>, indexed with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and number <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>GukiZiana</i>(<i>a</i>, <i>y</i>)</span> represents maximum value of <span class="tex-span"><i>j</i> - <i>i</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> = <i>y</i></span>. If there is no <span class="tex-span"><i>y</i></span> as an element in <span class="tex-span"><i>a</i></span>, then <span class="tex-span"><i>GukiZiana</i>(<i>a</i>, <i>y</i>)</span> is equal to <span class="tex-span"> - 1</span>. GukiZ also prepared a problem for you. This time, you have two types of queries: </p><ol> <li> First type has form <span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> and asks you to increase values of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> by the non-negative integer <span class="tex-span"><i>x</i></span>. </li><li> Second type has form <span class="tex-span">2</span> <span class="tex-span"><i>y</i></span> and asks you to find value of <span class="tex-span"><i>GukiZiana</i>(<i>a</i>, <i>y</i>)</span>. </li></ol><p>For each query of type <span class="tex-span">2</span>, print the answer and make GukiZ happy!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5 * 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 5 * 10<sup class="upper-index">4</sup></span>), size of array <span class="tex-span"><i>a</i></span>, and the number of queries. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), forming an array <span class="tex-span"><i>a</i></span>. </p><p>Each of next <span class="tex-span"><i>q</i></span> lines contain either four or two numbers, as described in statement:</p><p>If line starts with <span class="tex-span">1</span>, then the query looks like <span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>), first type query.</p><p>If line starts with <span class="tex-span">2</span>, then th query looks like <span class="tex-span">2</span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>), second type query.</p></div><div class="output-specification"><p>For each query of type <span class="tex-span">2</span>, print the value of <span class="tex-span"><i>GukiZiana</i>(<i>a</i>, <i>y</i>)</span>, for <span class="tex-span"><i>y</i></span> value for that query.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5 * 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 5 * 10<sup class="upper-index">4</sup></span>), size of array <span class="tex-span"><i>a</i></span>, and the number of queries. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), forming an array <span class="tex-span"><i>a</i></span>. </p><p>Each of next <span class="tex-span"><i>q</i></span> lines contain either four or two numbers, as described in statement:</p><p>If line starts with <span class="tex-span">1</span>, then the query looks like <span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>), first type query.</p><p>If line starts with <span class="tex-span">2</span>, then th query looks like <span class="tex-span">2</span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>), second type query.</p>

## Output

<p>For each query of type <span class="tex-span">2</span>, print the value of <span class="tex-span"><i>GukiZiana</i>(<i>a</i>, <i>y</i>)</span>, for <span class="tex-span"><i>y</i></span> value for that query.</p>





```input1
4 3
1 2 3 4
1 1 2 1
1 1 1 1
2 3

```




```input2
2 3
1 2
1 2 2 1
2 3
2 4

```




```output1
2

```




```output2
0
-1

```


