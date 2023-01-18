## Description

<div><p>You are given an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>m</i></span> sets <span class="tex-span"><i>S</i><sub class="lower-index">1</sub>, <i>S</i><sub class="lower-index">2</sub>, ..., <i>S</i><sub class="lower-index"><i>m</i></sub></span> of indices of elements of this array. Let's denote <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub> = {<i>S</i><sub class="lower-index"><i>k</i>, <i>i</i></sub>}&nbsp;(1 ≤ <i>i</i> ≤ |<i>S</i><sub class="lower-index"><i>k</i></sub>|)</span>. In other words, <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i>, <i>i</i></sub></span> is some element from set <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>In this problem you have to answer <span class="tex-span"><i>q</i></span> queries of the two types:</p><ol> <li> Find the sum of elements with indices from set <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span>: <img align="middle" class="tex-formula" src="file://a8HBQdKT.png" style="max-width: 100.0%;max-height: 100.0%;">. The query format is "<span class="tex-font-style-tt">? k</span>". </li><li> Add number <span class="tex-span"><i>x</i></span> to all elements at indices from set <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span>: <span class="tex-span"><i>a</i><sub class="lower-index"><i>S</i><sub class="lower-index"><i>k</i>, <i>i</i></sub></sub></span> is replaced by <span class="tex-span"><i>a</i><sub class="lower-index"><i>S</i><sub class="lower-index"><i>k</i>, <i>i</i></sub></sub> + <i>x</i></span> for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>S</i><sub class="lower-index"><i>k</i></sub>|)</span>. The query format is "<span class="tex-font-style-tt">+ k x</span>". </li></ol><p>After each first type query print the required sum.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">8</sup>)</span> — elements of array <span class="tex-span"><i>a</i></span>. </p><p>Each of the following <span class="tex-span"><i>m</i></span> lines describes one set of indices. The <span class="tex-span"><i>k</i></span>-th line first contains a positive integer, representing the number of elements in set (<span class="tex-span">|<i>S</i><sub class="lower-index"><i>k</i></sub>|</span>), then follow <span class="tex-span">|<i>S</i><sub class="lower-index"><i>k</i></sub>|</span> distinct integers <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i>, 1</sub>, <i>S</i><sub class="lower-index"><i>k</i>, 2</sub>, ..., <i>S</i><sub class="lower-index"><i>k</i>, |<i>S</i><sub class="lower-index"><i>k</i></sub>|</sub></span> <span class="tex-span">(1 ≤ <i>S</i><sub class="lower-index"><i>k</i>, <i>i</i></sub> ≤ <i>n</i>)</span> — elements of set <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain queries. Each query looks like either "<span class="tex-font-style-tt">? k</span>" or "<span class="tex-font-style-tt">+ k x</span>" and sits on a single line. For all queries the following limits are held: <span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i></span>, <span class="tex-span">|<i>x</i>| ≤ 10<sup class="upper-index">8</sup></span>. The queries are given in order they need to be answered.</p><p>It is guaranteed that the sum of sizes of all sets <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>After each first type query print the required sum on a single line.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">8</sup>)</span> — elements of array <span class="tex-span"><i>a</i></span>. </p><p>Each of the following <span class="tex-span"><i>m</i></span> lines describes one set of indices. The <span class="tex-span"><i>k</i></span>-th line first contains a positive integer, representing the number of elements in set (<span class="tex-span">|<i>S</i><sub class="lower-index"><i>k</i></sub>|</span>), then follow <span class="tex-span">|<i>S</i><sub class="lower-index"><i>k</i></sub>|</span> distinct integers <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i>, 1</sub>, <i>S</i><sub class="lower-index"><i>k</i>, 2</sub>, ..., <i>S</i><sub class="lower-index"><i>k</i>, |<i>S</i><sub class="lower-index"><i>k</i></sub>|</sub></span> <span class="tex-span">(1 ≤ <i>S</i><sub class="lower-index"><i>k</i>, <i>i</i></sub> ≤ <i>n</i>)</span> — elements of set <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain queries. Each query looks like either "<span class="tex-font-style-tt">? k</span>" or "<span class="tex-font-style-tt">+ k x</span>" and sits on a single line. For all queries the following limits are held: <span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i></span>, <span class="tex-span">|<i>x</i>| ≤ 10<sup class="upper-index">8</sup></span>. The queries are given in order they need to be answered.</p><p>It is guaranteed that the sum of sizes of all sets <span class="tex-span"><i>S</i><sub class="lower-index"><i>k</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>After each first type query print the required sum on a single line.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 3 5
5 -5 5 1 -4
2 1 2
4 2 1 4 5
2 2 5
? 2
+ 3 4
? 1
+ 2 1
? 2

```




```output1
-3
4
9

```


