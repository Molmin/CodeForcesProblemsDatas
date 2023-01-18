## Description

<div><p>Gargari is jealous that his friend Caisa won the game from the previous problem. He wants to prove that he is a genius.</p><p>He has a <span class="tex-span"><i>n</i> × <i>n</i></span> chessboard. Each cell of the chessboard has a number written on it. Gargari wants to place two bishops on the chessboard in such a way that there is no cell that is attacked by both of them. Consider a cell with number <span class="tex-span"><i>x</i></span> written on it, if this cell is attacked by one of the bishops Gargari will get <span class="tex-span"><i>x</i></span> dollars for it. Tell Gargari, how to place bishops on the chessboard to get maximum amount of money.</p><p>We assume a cell is attacked by a bishop, if the cell is located on the same diagonal with the bishop (the cell, where the bishop is, also considered attacked by it).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2000)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — description of the chessboard.</p></div><div class="output-specification"><p>On the first line print the maximal number of dollars Gargari will get. On the next line print four integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the number of the row where the <span class="tex-span"><i>i</i></span>-th bishop should be placed, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is the number of the column where the <span class="tex-span"><i>i</i></span>-th bishop should be placed. Consider rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, and columns are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right.</p><p>If there are several optimal solutions, you can print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2000)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — description of the chessboard.</p>

## Output

<p>On the first line print the maximal number of dollars Gargari will get. On the next line print four integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the number of the row where the <span class="tex-span"><i>i</i></span>-th bishop should be placed, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is the number of the column where the <span class="tex-span"><i>i</i></span>-th bishop should be placed. Consider rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, and columns are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right.</p><p>If there are several optimal solutions, you can print any of them.</p>





```input1
4
1 1 1 1
2 1 1 0
1 1 1 0
1 0 0 1

```




```output1
12
2 2 3 2

```


