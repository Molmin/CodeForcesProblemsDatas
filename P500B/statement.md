## Description

<div><p>User ainta has a permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. As the New Year is coming, he wants to make his permutation as pretty as possible.</p><p>Permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is <span class="tex-font-style-it">prettier</span> than permutation <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, if and only if there exists an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>b</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub> = <i>b</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i> - 1</sub> = <i>b</i><sub class="lower-index"><i>k</i> - 1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> &lt; <i>b</i><sub class="lower-index"><i>k</i></sub></span> all holds.</p><p>As known, permutation <span class="tex-span"><i>p</i></span> is so sensitive that it could be only modified by swapping two distinct elements. But swapping two elements is harder than you think. Given an <span class="tex-span"><i>n</i> × <i>n</i></span> binary matrix <span class="tex-span"><i>A</i></span>, user ainta can swap the values of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>) if and only if <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span>.</p><p>Given the permutation <span class="tex-span"><i>p</i></span> and the matrix <span class="tex-span"><i>A</i></span>, user ainta wants to know the prettiest permutation that he can obtain.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the size of the permutation <span class="tex-span"><i>p</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the permutation <span class="tex-span"><i>p</i></span> that user ainta has. Each integer between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> occurs exactly once in the given permutation.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the matrix <span class="tex-span"><i>A</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' and describes the <span class="tex-span"><i>i</i></span>-th row of <span class="tex-span"><i>A</i></span>. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is the element on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column of A. It is guaranteed that, for all integers <span class="tex-span"><i>i</i>, <i>j</i></span> where <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>A</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> holds. Also, for all integers <span class="tex-span"><i>i</i></span> where <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span> holds.</p></div><div class="output-specification"><p>In the first and only line, print <span class="tex-span"><i>n</i></span> space-separated integers, describing the prettiest permutation that can be obtained.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the size of the permutation <span class="tex-span"><i>p</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the permutation <span class="tex-span"><i>p</i></span> that user ainta has. Each integer between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> occurs exactly once in the given permutation.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the matrix <span class="tex-span"><i>A</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' and describes the <span class="tex-span"><i>i</i></span>-th row of <span class="tex-span"><i>A</i></span>. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is the element on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column of A. It is guaranteed that, for all integers <span class="tex-span"><i>i</i>, <i>j</i></span> where <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>A</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> holds. Also, for all integers <span class="tex-span"><i>i</i></span> where <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span> holds.</p>

## Output

<p>In the first and only line, print <span class="tex-span"><i>n</i></span> space-separated integers, describing the prettiest permutation that can be obtained.</p>





```input1
7
5 2 4 3 6 7 1
0001001
0000000
0000010
1000001
0000000
0010000
1001000

```




```input2
5
4 2 1 5 3
00100
00011
10010
01101
01010

```




```output1
1 2 4 3 6 7 5

```




```output2
1 2 3 4 5

```



## Note

<p>In the first sample, the swap needed to obtain the prettiest permutation is: <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">7</sub>)</span>.</p><p>In the second sample, the swaps needed to obtain the prettiest permutation is <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">3</sub>), (<i>p</i><sub class="lower-index">4</sub>, <i>p</i><sub class="lower-index">5</sub>), (<i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub>)</span>. </p><center> <img class="tex-graphics" src="file://uS2R4PAk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A <span class="tex-font-style-bf">permutation</span> <span class="tex-span"><i>p</i></span> is a sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each of them doesn't exceed <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th element of the permutation <span class="tex-span"><i>p</i></span> is denoted as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. The size of the permutation <span class="tex-span"><i>p</i></span> is denoted as <span class="tex-span"><i>n</i></span>.</p>
