## Description

<div><p>Bob has a favorite number <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>n</i></span>. Now he asks you to answer <span class="tex-span"><i>m</i></span> queries. Each query is given by a pair <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and asks you to count the number of pairs of integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>j</i> ≤ <i>r</i></span> and the xor of the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>j</i></sub></span> is equal to <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 1 000 000</span>)&nbsp;— the length of the array, the number of queries and Bob's favorite number respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— Bob's array.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the parameters of the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, answer the queries in the order they appear in the input. </p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 1 000 000</span>)&nbsp;— the length of the array, the number of queries and Bob's favorite number respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— Bob's array.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the parameters of the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, answer the queries in the order they appear in the input. </p>





```input1
6 2 3
1 2 1 1 0 3
1 6
3 5

```




```input2
5 3 1
1 1 1 1 1
1 5
2 4
1 3

```




```output1
7
0

```




```output2
9
4
4

```



## Note

<p>In the first sample the suitable pairs of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> for the first query are: (<span class="tex-span">1</span>, <span class="tex-span">2</span>), (<span class="tex-span">1</span>, <span class="tex-span">4</span>), (<span class="tex-span">1</span>, <span class="tex-span">5</span>), (<span class="tex-span">2</span>, <span class="tex-span">3</span>), (<span class="tex-span">3</span>, <span class="tex-span">6</span>), (<span class="tex-span">5</span>, <span class="tex-span">6</span>), (<span class="tex-span">6</span>, <span class="tex-span">6</span>). Not a single of these pairs is suitable for the second query.</p><p>In the second sample xor equals <span class="tex-span">1</span> for all subarrays of an odd length.</p>
