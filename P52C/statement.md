## Description

<div><p>You are given circular array <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>. There are two types of operations with it: </p><ul> <li> <span class="tex-span"><i>inc</i>(<i>lf</i>, <i>rg</i>, <i>v</i>)</span> — this operation increases each element on the segment <span class="tex-span">[<i>lf</i>, <i>rg</i>]</span> (inclusively) by <span class="tex-span"><i>v</i></span>; </li><li> <span class="tex-span"><i>rmq</i>(<i>lf</i>, <i>rg</i>)</span> — this operation returns minimal value on the segment <span class="tex-span">[<i>lf</i>, <i>rg</i>]</span> (inclusively). </li></ul><p>Assume segments to be circular, so if <span class="tex-span"><i>n</i> = 5</span> and <span class="tex-span"><i>lf</i> = 3, <i>rg</i> = 1</span>, it means the index sequence: <span class="tex-span">3, 4, 0, 1</span>.</p><p>Write program to process given sequence of operations.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>). The next line contains initial state of the array: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are integer. The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 200000</span>), <span class="tex-span"><i>m</i></span> — the number of operartons. Next <span class="tex-span"><i>m</i></span> lines contain one operation each. If line contains two integer <span class="tex-span"><i>lf</i>, <i>rg</i></span> (<span class="tex-span">0 ≤ <i>lf</i>, <i>rg</i> ≤ <i>n</i> - 1</span>) it means <span class="tex-span"><i>rmq</i></span> operation, it contains three integers <span class="tex-span"><i>lf</i>, <i>rg</i>, <i>v</i></span> (<span class="tex-span">0 ≤ <i>lf</i>, <i>rg</i> ≤ <i>n</i> - 1; - 10<sup class="upper-index">6</sup> ≤ <i>v</i> ≤ 10<sup class="upper-index">6</sup></span>) — <span class="tex-span"><i>inc</i></span> operation.</p></div><div class="output-specification"><p>For each <span class="tex-span"><i>rmq</i></span> operation write result for it. Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>). The next line contains initial state of the array: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are integer. The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 200000</span>), <span class="tex-span"><i>m</i></span> — the number of operartons. Next <span class="tex-span"><i>m</i></span> lines contain one operation each. If line contains two integer <span class="tex-span"><i>lf</i>, <i>rg</i></span> (<span class="tex-span">0 ≤ <i>lf</i>, <i>rg</i> ≤ <i>n</i> - 1</span>) it means <span class="tex-span"><i>rmq</i></span> operation, it contains three integers <span class="tex-span"><i>lf</i>, <i>rg</i>, <i>v</i></span> (<span class="tex-span">0 ≤ <i>lf</i>, <i>rg</i> ≤ <i>n</i> - 1; - 10<sup class="upper-index">6</sup> ≤ <i>v</i> ≤ 10<sup class="upper-index">6</sup></span>) — <span class="tex-span"><i>inc</i></span> operation.</p>

## Output

<p>For each <span class="tex-span"><i>rmq</i></span> operation write result for it. Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
4
1 2 3 4
4
3 0
3 0 -1
0 1
2 1

```




```output1
1
0
0

```


