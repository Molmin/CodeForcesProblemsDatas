## Description

<div><p>You are given array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> integers and <span class="tex-span"><i>m</i></span> queries. The <span class="tex-span"><i>i</i></span>-th query is given with three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>For the <span class="tex-span"><i>i</i></span>-th query find any position <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>) so that <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub> ≠ <i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in <span class="tex-span"><i>a</i></span> and the number of queries.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the parameters of the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th line print integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the position of any number not equal to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> in segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> or the value <span class="tex-span"> - 1</span> if there is no such number.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in <span class="tex-span"><i>a</i></span> and the number of queries.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the parameters of the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th line print integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the position of any number not equal to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> in segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> or the value <span class="tex-span"> - 1</span> if there is no such number.</p>





```input1
6 4
1 2 1 1 3 5
1 4 1
2 6 2
3 4 1
3 4 2

```




```output1
2
6
-1
4

```


