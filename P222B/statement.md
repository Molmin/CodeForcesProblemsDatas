## Description

<div><p>The Free Meteor Association (FMA) has got a problem: as meteors are moving, the Universal Cosmic Descriptive Humorous Program (UCDHP) needs to add a special module that would analyze this movement. </p><p>UCDHP stores some secret information about meteors as an <span class="tex-span"><i>n</i> × <i>m</i></span> table with integers in its cells. The order of meteors in the Universe is changing. That's why the main UCDHP module receives the following queries:</p><ul> <li> The query to swap two table rows; </li><li> The query to swap two table columns; </li><li> The query to obtain a secret number in a particular table cell. </li></ul><p>As the main UCDHP module is critical, writing the functional of working with the table has been commissioned to you.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 500000</span>) — the number of table columns and rows and the number of queries, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> space-separated numbers each — the initial state of the table. Each number <span class="tex-span"><i>p</i></span> in the table is an integer and satisfies the inequality <span class="tex-span">0 ≤ <i>p</i> ≤ 10<sup class="upper-index">6</sup></span>.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain queries in the format "<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is one of the characters "<span class="tex-font-style-tt">с</span>", "<span class="tex-font-style-tt">r</span>" or "<span class="tex-font-style-tt">g</span>", and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are two integers.</p><ul> <li> If <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">c</span>", then the current query is the query to swap columns with indexes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>m</i>, <i>x</i> ≠ <i>y</i></span>); </li><li> If <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">r</span>", then the current query is the query to swap rows with indexes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>); </li><li> If <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">g</span>", then the current query is the query to obtain the number that located in the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th row and in the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th column (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>). </li></ul><p>The table rows are considered to be indexed from top to bottom from 1 to <span class="tex-span"><i>n</i></span>, and the table columns — from left to right from 1 to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>For each query to obtain a number (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">g</span>") print the required number. Print the answers to the queries in the order of the queries in the input.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 500000</span>) — the number of table columns and rows and the number of queries, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> space-separated numbers each — the initial state of the table. Each number <span class="tex-span"><i>p</i></span> in the table is an integer and satisfies the inequality <span class="tex-span">0 ≤ <i>p</i> ≤ 10<sup class="upper-index">6</sup></span>.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain queries in the format "<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is one of the characters "<span class="tex-font-style-tt">с</span>", "<span class="tex-font-style-tt">r</span>" or "<span class="tex-font-style-tt">g</span>", and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are two integers.</p><ul> <li> If <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">c</span>", then the current query is the query to swap columns with indexes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>m</i>, <i>x</i> ≠ <i>y</i></span>); </li><li> If <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">r</span>", then the current query is the query to swap rows with indexes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>); </li><li> If <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">g</span>", then the current query is the query to obtain the number that located in the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th row and in the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th column (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>). </li></ul><p>The table rows are considered to be indexed from top to bottom from 1 to <span class="tex-span"><i>n</i></span>, and the table columns — from left to right from 1 to <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>For each query to obtain a number (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">g</span>") print the required number. Print the answers to the queries in the order of the queries in the input.</p>





```input1
3 3 5
1 2 3
4 5 6
7 8 9
g 3 2
r 3 2
c 2 3
g 2 2
g 3 2

```




```input2
2 3 3
1 2 4
3 1 5
c 2 1
r 1 2
g 1 3

```




```output1
8
9
6

```




```output2
5

```



## Note

<p>Let's see how the table changes in the second test case.</p><p>After the first operation is fulfilled, the table looks like that:</p><p>2 1 4</p><p>1 3 5</p><p>After the second operation is fulfilled, the table looks like that:</p><p>1 3 5</p><p>2 1 4</p><p>So the answer to the third query (the number located in the first row and in the third column) will be 5.</p>
