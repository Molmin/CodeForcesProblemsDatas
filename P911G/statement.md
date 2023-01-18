## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. You have to process <span class="tex-span"><i>q</i></span> queries to this array; each query is given as four numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, denoting that for every <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>x</i></span> you have to set <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equal to <span class="tex-span"><i>y</i></span>.</p><p>Print the array after all queries are processed.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the size of array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of array <span class="tex-span"><i>a</i></span>.</p><p>The third line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200000</span>) — the number of queries you have to process.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. <span class="tex-span"><i>i</i></span>-th line contains four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> denoting <span class="tex-span"><i>i</i></span>-th query (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers — elements of array <span class="tex-span"><i>a</i></span> after all changes are made.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the size of array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of array <span class="tex-span"><i>a</i></span>.</p><p>The third line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200000</span>) — the number of queries you have to process.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. <span class="tex-span"><i>i</i></span>-th line contains four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> denoting <span class="tex-span"><i>i</i></span>-th query (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 100</span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers — elements of array <span class="tex-span"><i>a</i></span> after all changes are made.</p>





```input1
5
1 2 3 4 5
3
3 5 3 5
1 5 5 1
1 5 1 5

```




```output1
5 2 5 4 5
```


