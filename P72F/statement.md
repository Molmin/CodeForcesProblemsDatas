## Description

<div><p>After the nationalization of the oil industry, Dr. Mosaddegh wants to dig some oil wells to extract all the oil in Persian Gulf. But Persian Gulf is huge and has an infinite amount of oil. So Dr. Mosaddegh works only on a rectangular plane of size <span class="tex-span"><i>n</i> × <i>m</i></span> of the Persian Gulf. Each of the cells in this rectangle either contains an infinite amount of oil or nothing.</p><p>Two cells are considered adjacent if and only if they have a common edge, a path is a sequence <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>x</i></sub></span> of cells so that all of them contain oil and for each <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is adjacent to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> - 1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> (if they exist). Two cells are considered <span class="tex-font-style-underline">connected</span> to each other if and only if there exists a path between them. If we dig a well in a certain cell, we can extract oil from all the cells that are <span class="tex-font-style-underline">connected</span> to it by oil paths. It is not allowed to dig wells on empty cells.</p><p>Dr. Mosaddegh also knows that in Persian Gulf, the empty cells form rows and columns. I. e. if some cell is empty, then it's column is completely empty or it's row is completely empty, or both.</p><p>Help Dr. Mosaddegh find out how many wells he has to dig to access all the oil in that region.</p></div><div class="input-specification"><p>In the first line there are two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p><p>In the second line there is an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 ≤ <i>t</i> ≤ <i>n</i></span>), the number of empty rows. <span class="tex-span"><i>t</i></span> distinct positive integers follow, these are the numbers of empty rows and are in range <span class="tex-span">[1, <i>n</i>]</span>.</p><p>In the second line there is an integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">0 ≤ <i>s</i> ≤ <i>m</i></span>) that shows the number of columns not having any oil. <span class="tex-span"><i>s</i></span> distinct positive integers follow, these are the numbers of empty columns and are in range of <span class="tex-span">[1, <i>m</i>]</span>.</p><p>Note that rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (from top to bottom) and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> (from left to right).</p></div><div class="output-specification"><p>A single integer, the minimum number of wells that Dr. Mossadegh has to dig.</p><p>This is actually finding how many regions are made by removing the given rows and columns.</p></div>

## Input

<p>In the first line there are two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p><p>In the second line there is an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 ≤ <i>t</i> ≤ <i>n</i></span>), the number of empty rows. <span class="tex-span"><i>t</i></span> distinct positive integers follow, these are the numbers of empty rows and are in range <span class="tex-span">[1, <i>n</i>]</span>.</p><p>In the second line there is an integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">0 ≤ <i>s</i> ≤ <i>m</i></span>) that shows the number of columns not having any oil. <span class="tex-span"><i>s</i></span> distinct positive integers follow, these are the numbers of empty columns and are in range of <span class="tex-span">[1, <i>m</i>]</span>.</p><p>Note that rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (from top to bottom) and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> (from left to right).</p>

## Output

<p>A single integer, the minimum number of wells that Dr. Mossadegh has to dig.</p><p>This is actually finding how many regions are made by removing the given rows and columns.</p>





```input1
2 3
1 2
1 2

```




```input2
4 4
2 2 3
3 2 3 1

```




```input3
2 3
1 1
0

```




```output1
2

```




```output2
2

```




```output3
1

```


