## Description

<div><p>The Smart Beaver from ABBYY began to develop a new educational game for children. The rules of the game are fairly simple and are described below.</p><p>The playing field is a sequence of <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The goal of the game is to make numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (i.e. some prefix of the sequence) equal to zero for some fixed <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &lt; <i>n</i>)</span>, and this should be done in the smallest possible number of moves.</p><p>One move is choosing an integer <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> and an integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(<i>t</i> ≥ 0)</span> such that <span class="tex-span"><i>i</i> + 2<sup class="upper-index"><i>t</i></sup> ≤ <i>n</i></span>. After the values of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>t</i></span> have been selected, the value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is decreased by <span class="tex-span">1</span>, and the value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 2<sup class="upper-index"><i>t</i></sup></sub></span> is increased by <span class="tex-span">1</span>. For example, let <span class="tex-span"><i>n</i> = 4</span> and <span class="tex-span"><i>a</i> = (1, 0, 1, 2)</span>, then it is possible to make move <span class="tex-span"><i>i</i> = 3</span>, <span class="tex-span"><i>t</i> = 0</span> and get <span class="tex-span"><i>a</i> = (1, 0, 0, 3)</span> or to make move <span class="tex-span"><i>i</i> = 1</span>, <span class="tex-span"><i>t</i> = 1</span> and get <span class="tex-span"><i>a</i> = (0, 0, 2, 2)</span> (the only possible other move is <span class="tex-span"><i>i</i> = 1</span>, <span class="tex-span"><i>t</i> = 0</span>).</p><p>You are given <span class="tex-span"><i>n</i></span> and the initial sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The task is to calculate the minimum number of moves needed to make the first <span class="tex-span"><i>k</i></span> elements of the original sequence equal to zero for each possible <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> &lt; <i>n</i>)</span>.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), separated by single spaces.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 300</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span> </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> </li></ul></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>n</i> - 1</span> lines: the <span class="tex-span"><i>k</i></span>-th output line must contain the minimum number of moves needed to make the first <span class="tex-span"><i>k</i></span> elements of the original sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equal to zero.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams, or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), separated by single spaces.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 300</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span> </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> </li></ul>

## Output

<p>Print exactly <span class="tex-span"><i>n</i> - 1</span> lines: the <span class="tex-span"><i>k</i></span>-th output line must contain the minimum number of moves needed to make the first <span class="tex-span"><i>k</i></span> elements of the original sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equal to zero.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams, or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4
1 0 1 2

```




```input2
8
1 2 3 4 5 6 7 8

```




```output1
1
1
3

```




```output2
1
3
6
10
16
24
40

```


