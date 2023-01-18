## Description

<div><p>You've got an array consisting of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span>. Moreover, there are <span class="tex-span"><i>m</i></span> queries, each query can be described by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span>. Query <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span> means that we should add <img align="middle" class="tex-formula" src="file://vMKtGkZA.png" style="max-width: 100.0%;max-height: 100.0%;"> to each element <span class="tex-span"><i>a</i>[<i>j</i>]</span>, where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>j</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Record <img align="middle" class="tex-formula" src="file://wD7IsnuO.png" style="max-width: 100.0%;max-height: 100.0%;"> means the binomial coefficient, or the number of combinations from <span class="tex-span"><i>y</i></span> elements into groups of <span class="tex-span"><i>x</i></span> elements.</p><p>You need to fulfil consecutively all queries and then print the final array.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the initial array.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain queries in the format <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— to all elements of the segment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>... <i>r</i><sub class="lower-index"><i>i</i></sub></span> add number <img align="middle" class="tex-formula" src="file://WyHwOuj8.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers: the <span class="tex-span"><i>i</i></span>-th number is the value of element <span class="tex-span"><i>a</i>[<i>i</i>]</span> after all the queries. As the values can be rather large, print them modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the initial array.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain queries in the format <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— to all elements of the segment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>... <i>r</i><sub class="lower-index"><i>i</i></sub></span> add number <img align="middle" class="tex-formula" src="file://WyHwOuj8.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers: the <span class="tex-span"><i>i</i></span>-th number is the value of element <span class="tex-span"><i>a</i>[<i>i</i>]</span> after all the queries. As the values can be rather large, print them modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
5 1
0 0 0 0 0
1 5 0

```




```input2
10 2
1 2 3 4 5 0 0 0 0 0
1 6 1
6 10 2

```




```output1
1 1 1 1 1

```




```output2
2 4 6 8 10 7 3 6 10 15

```


