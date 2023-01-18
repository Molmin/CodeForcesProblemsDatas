## Description

<div><p>Vasya has recently started to learn English. Now he needs to remember how to write English letters. He isn't sure about some of them, so he decided to train a little.</p><p>He found a sheet of squared paper and began writing arbitrary English letters there. In the end Vasya wrote <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each. Thus, he got a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span> table, each cell of the table contained some English letter. Let's number the table rows from top to bottom with integers from 1 to <span class="tex-span"><i>n</i></span>, and columns — from left to right with integers from 1 to <span class="tex-span"><i>m</i></span>.</p><p>After that Vasya looked at the resulting rectangular table and wondered, how many subtables are there, that matches both following conditions:</p><ul> <li> the subtable contains at most <span class="tex-span"><i>k</i></span> cells with "<span class="tex-font-style-tt">a</span>" letter; </li><li> all letters, located in all four corner cells of the subtable, are equal. </li></ul> <p>Formally, a subtable's definition is as follows. It is defined by four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> such that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>. Then the subtable contains all such cells <span class="tex-span">(<i>x</i>, <i>y</i>)</span> (<span class="tex-span"><i>x</i></span> is the row number, <span class="tex-span"><i>y</i></span> is the column number), for which the following inequality holds <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub></span>. The corner cells of the table are cells <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>Vasya is already too tired after he's been writing letters to a piece of paper. That's why he asks you to count the value he is interested in.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 400;&nbsp;0 ≤ <i>k</i> ≤ <i>n</i>·<i>m</i>)</span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the given table. Each character of the table is a lowercase English letter.</p></div><div class="output-specification"><p>Print a single integer — the number of required subtables.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 400;&nbsp;0 ≤ <i>k</i> ≤ <i>n</i>·<i>m</i>)</span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the given table. Each character of the table is a lowercase English letter.</p>

## Output

<p>Print a single integer — the number of required subtables.</p>





```input1
3 4 4
aabb
baab
baab

```




```input2
4 5 1
ababa
ccaca
ccacb
cbabc

```




```output1
2

```




```output2
1

```



## Note

<p>There are two suitable subtables in the first sample: the first one's upper left corner is cell <span class="tex-span">(2, 2)</span> and lower right corner is cell <span class="tex-span">(3, 3)</span>, the second one's upper left corner is cell <span class="tex-span">(2, 1)</span> and lower right corner is cell <span class="tex-span">(3, 4)</span>.</p>
