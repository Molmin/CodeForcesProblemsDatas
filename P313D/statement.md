## Description

<div><p>Everything is great about Ilya's city, except the roads. The thing is, the only ZooVille road is represented as <span class="tex-span"><i>n</i></span> holes in a row. We will consider the holes numbered from 1 to <span class="tex-span"><i>n</i></span>, from left to right.</p><p>Ilya is really keep on helping his city. So, he wants to fix at least <span class="tex-span"><i>k</i></span> holes (perharps he can fix more) on a single ZooVille road. </p><p>The city has <span class="tex-span"><i>m</i></span> building companies, the <span class="tex-span"><i>i</i></span>-th company needs <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> money units to fix a road segment containing holes with numbers of at least <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and at most <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. The companies in ZooVille are very greedy, so, if they fix a segment containing some already fixed holes, they do not decrease the price for fixing the segment. </p><p>Determine the minimum money Ilya will need to fix at least <span class="tex-span"><i>k</i></span> holes.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i>)</span>. The next <span class="tex-span"><i>m</i></span> lines contain the companies' description. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum money Ilya needs to fix at least <span class="tex-span"><i>k</i></span> holes. </p><p>If it is impossible to fix at least <span class="tex-span"><i>k</i></span> holes, print <span class="tex-font-style-tt">-1</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i>)</span>. The next <span class="tex-span"><i>m</i></span> lines contain the companies' description. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print a single integer — the minimum money Ilya needs to fix at least <span class="tex-span"><i>k</i></span> holes. </p><p>If it is impossible to fix at least <span class="tex-span"><i>k</i></span> holes, print <span class="tex-font-style-tt">-1</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
10 4 6
7 9 11
6 9 13
7 7 7
3 5 6

```




```input2
10 7 1
3 4 15
8 9 8
5 6 8
9 10 6
1 4 2
1 4 10
8 10 13

```




```input3
10 1 9
5 10 14

```




```output1
17

```




```output2
2

```




```output3
-1

```


