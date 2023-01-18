## Description

<div><p>You've got table <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> rows, numbered from 1 to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th line of table <span class="tex-span"><i>a</i></span> contains <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> cells, at that for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 &lt; <i>i</i> ≤ <i>n</i>)</span> holds <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i> - 1</sub></span>. </p><p>Let's denote <span class="tex-span"><i>s</i></span> as the total number of cells of table <span class="tex-span"><i>a</i></span>, that is, <img align="middle" class="tex-formula" src="file://IdyHNzy7.png" style="max-width: 100.0%;max-height: 100.0%;">. We know that each cell of the table contains a single integer from <span class="tex-span">1</span> to <span class="tex-span"><i>s</i></span>, at that all written integers are distinct. </p><p>Let's assume that the cells of the <span class="tex-span"><i>i</i></span>-th row of table <span class="tex-span"><i>a</i></span> are numbered from 1 to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, then let's denote the number written in the <span class="tex-span"><i>j</i></span>-th cell of the <span class="tex-span"><i>i</i></span>-th row as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. Your task is to perform several swap operations to rearrange the numbers in the table so as to fulfill the following conditions:</p><ol> <li> for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 &lt; <i>i</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>j</i> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>)</span> holds <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i> - 1, <i>j</i></sub></span>; </li><li> for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>;&nbsp;1 &lt; <i>j</i> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>)</span> holds <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i> - 1</sub></span>. </li></ol><p>In one swap operation you are allowed to choose two different cells of the table and swap the recorded there numbers, that is the number that was recorded in the first of the selected cells before the swap, is written in the second cell after it. Similarly, the number that was recorded in the second of the selected cells, is written in the first cell after the swap.</p><p>Rearrange the numbers in the required manner. Note that you are allowed to perform any number of operations, but not more than <span class="tex-span"><i>s</i></span>. You do not have to minimize the number of operations.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> that shows the number of rows in the table. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 50;&nbsp;<i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i> - 1</sub>)</span> — the numbers of cells on the corresponding rows.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain table <span class="tex-span"><i>а</i></span>. The <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers: the <span class="tex-span"><i>j</i></span>-th integer in this line represents <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>.</p><p>It is guaranteed that all the given numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are positive and do not exceed <span class="tex-span"><i>s</i></span>. It is guaranteed that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are distinct.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ <i>s</i>)</span>, representing the number of performed swaps.</p><p>In the next <span class="tex-span"><i>m</i></span> lines print the description of these swap operations. In the <span class="tex-span"><i>i</i></span>-th line print four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub></sub>;&nbsp;1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub>)</span>. The printed numbers denote swapping the contents of cells <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></sub></span>. Note that a swap operation can change the contents of <span class="tex-font-style-bf">distinct</span> table cells. Print the swaps in the order, in which they should be executed.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> that shows the number of rows in the table. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 50;&nbsp;<i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i> - 1</sub>)</span> — the numbers of cells on the corresponding rows.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain table <span class="tex-span"><i>а</i></span>. The <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers: the <span class="tex-span"><i>j</i></span>-th integer in this line represents <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>.</p><p>It is guaranteed that all the given numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are positive and do not exceed <span class="tex-span"><i>s</i></span>. It is guaranteed that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are distinct.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ <i>s</i>)</span>, representing the number of performed swaps.</p><p>In the next <span class="tex-span"><i>m</i></span> lines print the description of these swap operations. In the <span class="tex-span"><i>i</i></span>-th line print four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub></sub>;&nbsp;1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub>)</span>. The printed numbers denote swapping the contents of cells <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></sub></span>. Note that a swap operation can change the contents of <span class="tex-font-style-bf">distinct</span> table cells. Print the swaps in the order, in which they should be executed.</p>





```input1
3
3 2 1
4 3 5
6 1
2

```




```input2
1
4
4 3 2 1

```




```output1
2
1 1 2 2
2 1 3 1

```




```output2
2
1 1 1 4
1 2 1 3

```


