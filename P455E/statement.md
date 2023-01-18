## Description

<div><p>Serega and Fedor play with functions. One day they came across a very interesting function. It looks like that:</p><ul> <li> <span class="tex-span"><i>f</i>(1, <i>j</i>) = <i>a</i>[<i>j</i>]</span>, <span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>. </li><li> <span class="tex-span"><i>f</i>(<i>i</i>, <i>j</i>) = <i>min</i>(<i>f</i>(<i>i</i> - 1, <i>j</i>), <i>f</i>(<i>i</i> - 1, <i>j</i> - 1)) + <i>a</i>[<i>j</i>]</span>, <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-font-style-bf"><span class="tex-span"><i>i</i> ≤ <i>j</i> ≤ <i>n</i></span></span>. </li></ul><p>Here <span class="tex-span"><i>a</i></span> is an integer array of length <span class="tex-span"><i>n</i></span>.</p><p>Serega and Fedya want to know what values this function takes at some points. But they don't want to calculate the values manually. So they ask you to help them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of array <span class="tex-span"><i>a</i></span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Each line means that Fedor and Serega want to know the value of <span class="tex-span"><i>f</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines — the answers to the guys' queries.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of array <span class="tex-span"><i>a</i></span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Each line means that Fedor and Serega want to know the value of <span class="tex-span"><i>f</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines — the answers to the guys' queries.</p>





```input1
6
2 2 3 4 3 4
4
4 5
3 4
3 4
2 3

```




```input2
7
1 3 2 3 4 0 2
4
4 5
2 3
1 4
4 6

```




```output1
12
9
9
5

```




```output2
11
4
3
0

```


