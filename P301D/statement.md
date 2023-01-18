## Description

<div><p>Yaroslav has an array <span class="tex-span"><i>p</i> = <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, consisting of <span class="tex-span"><i>n</i></span> distinct integers. Also, he has <span class="tex-span"><i>m</i></span> queries:</p><ul> <li> Query number <span class="tex-span"><i>i</i></span> is represented as a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. </li><li> The answer to the query <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> is the number of pairs of integers <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>w</i></span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i>, <i>w</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>q</i></sub></span> is the divisor of <span class="tex-span"><i>p</i><sub class="lower-index"><i>w</i></sub></span>. </li></ul><p>Help Yaroslav, answer all his queries.</p></div><div class="input-specification"><p>The first line contains the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. The following <span class="tex-span"><i>m</i></span> lines contain Yaroslav's queries. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the answers to Yaroslav's queries in the order they appear in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. The following <span class="tex-span"><i>m</i></span> lines contain Yaroslav's queries. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the answers to Yaroslav's queries in the order they appear in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1 1
1
1 1

```




```input2
10 9
1 2 3 4 5 6 7 8 9 10
1 10
2 9
3 8
4 7
5 6
2 2
9 10
5 10
4 10

```




```output1
1

```




```output2
27
14
8
4
2
1
2
7
9

```


