## Description

<div><p>DZY has a hash table with <span class="tex-span"><i>p</i></span> buckets, numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>p</i> - 1</span>. He wants to insert <span class="tex-span"><i>n</i></span> numbers, in the order they are given, into the hash table. For the <span class="tex-span"><i>i</i></span>-th number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, DZY will put it into the bucket numbered <span class="tex-span"><i>h</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>)</span>, where <span class="tex-span"><i>h</i>(<i>x</i>)</span> is the hash function. In this problem we will assume, that <span class="tex-span"><i>h</i>(<i>x</i>) = <i>x</i>&nbsp;<i>mod</i>&nbsp;<i>p</i></span>. Operation <span class="tex-span"><i>a</i>&nbsp;<i>mod</i>&nbsp;<i>b</i></span> denotes taking a remainder after division <span class="tex-span"><i>a</i></span> by <span class="tex-span"><i>b</i></span>.</p><p>However, each bucket can contain no more than one element. If DZY wants to insert an number into a bucket which is already filled, we say a "conflict" happens. Suppose the first conflict happens right after the <span class="tex-span"><i>i</i></span>-th insertion, you should output <span class="tex-span"><i>i</i></span>. If no conflict happens, just output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>p</i>, <i>n</i> ≤ 300)</span>. Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>p</i>, <i>n</i> ≤ 300)</span>. Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output a single integer — the answer to the problem.</p>





```input1
10 5
0
21
53
41
53

```




```input2
5 5
0
1
2
3
4

```




```output1
4

```




```output2
-1

```


