## Description

<div><p><span class="tex-font-style-it">Mashmokh's boss, Bimokh, didn't like Mashmokh. So he fired him. Mashmokh decided to go to university and participate in ACM instead of finding a new job. He wants to become a member of Bamokh's team. In order to join he was given some programming tasks and one week to solve them. Mashmokh is not a very experienced programmer. Actually he is not a programmer at all. So he wasn't able to solve them. That's why he asked you to help him with these tasks. One of these tasks is the following.</span></p><p>You have an array <span class="tex-span"><i>a</i></span> of length <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> and <span class="tex-span"><i>m</i></span> queries on it. The <span class="tex-span"><i>i</i></span>-th query is described by an integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. In order to perform the <span class="tex-span"><i>i</i></span>-th query you must:</p><ul> <li> split the array into <span class="tex-span">2<sup class="upper-index"><i>n</i> - <i>q</i><sub class="lower-index"><i>i</i></sub></sup></span> parts, where each part is a subarray consisting of <span class="tex-span">2<sup class="upper-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sup></span> numbers; the <span class="tex-span"><i>j</i></span>-th subarray <span class="tex-span">(1 ≤ <i>j</i> ≤ 2<sup class="upper-index"><i>n</i> - <i>q</i><sub class="lower-index"><i>i</i></sub></sup>)</span> should contain the elements <span class="tex-span"><i>a</i>[(<i>j</i> - 1)·2<sup class="upper-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sup> + 1], <i>a</i>[(<i>j</i> - 1)·2<sup class="upper-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sup> + 2], ..., <i>a</i>[(<i>j</i> - 1)·2<sup class="upper-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sup> + 2<sup class="upper-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sup>]</span>; </li><li> reverse each of the subarrays; </li><li> join them into a single array in the same order (this array becomes new array <span class="tex-span"><i>a</i></span>); </li><li> output the number of inversions in the new <span class="tex-span"><i>a</i></span>. </li></ul><p>Given initial array <span class="tex-span"><i>a</i></span> and all the queries. Answer all the queries. Please, note that the changes from some query is saved for further queries.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i>&nbsp;(0 ≤ <i>n</i> ≤ 20)</span>. </p><p>The second line of input contains <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> space-separated integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[2<sup class="upper-index"><i>n</i></sup>]&nbsp;(1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>)</span>, the initial array.</p><p>The third line of input contains a single integer <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span>. </p><p>The fourth line of input contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>m</i></sub>&nbsp;(0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, the queries.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>m</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the answer (the number of inversions) for the <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i>&nbsp;(0 ≤ <i>n</i> ≤ 20)</span>. </p><p>The second line of input contains <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> space-separated integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[2<sup class="upper-index"><i>n</i></sup>]&nbsp;(1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>)</span>, the initial array.</p><p>The third line of input contains a single integer <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span>. </p><p>The fourth line of input contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>m</i></sub>&nbsp;(0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, the queries.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p>

## Output

<p>Output <span class="tex-span"><i>m</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the answer (the number of inversions) for the <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
2
2 1 4 3
4
1 2 0 2

```




```input2
1
1 2
3
0 1 1

```




```output1
0
6
6
0

```




```output2
0
1
0

```



## Note

<p>If we reverse an array <span class="tex-span"><i>x</i>[1], <i>x</i>[2], ..., <i>x</i>[<i>n</i>]</span> it becomes new array <span class="tex-span"><i>y</i>[1], <i>y</i>[2], ..., <i>y</i>[<i>n</i>]</span>, where <span class="tex-span"><i>y</i>[<i>i</i>] = <i>x</i>[<i>n</i> - <i>i</i> + 1]</span> for each <span class="tex-span"><i>i</i></span>.</p><p>The number of inversions of an array <span class="tex-span"><i>x</i>[1], <i>x</i>[2], ..., <i>x</i>[<i>n</i>]</span> is the number of pairs of indices <span class="tex-span"><i>i</i>, <i>j</i></span> such that: <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span"><i>x</i>[<i>i</i>] &gt; <i>x</i>[<i>j</i>]</span>.</p>
