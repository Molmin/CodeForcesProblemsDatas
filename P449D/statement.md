## Description

<div><p>Jzzhu have <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. We will call a sequence of indexes <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>)</span> a group of size <span class="tex-span"><i>k</i></span>. </p><p>Jzzhu wonders, how many groups exists such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub></span> &amp; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub></span> &amp; ... &amp; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub> = 0</span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i>)</span>? Help him and print this number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Operation <span class="tex-span"><i>x</i></span> &amp; <span class="tex-span"><i>y</i></span> denotes bitwise AND operation of two numbers.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>Output a single integer representing the number of required groups modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>Output a single integer representing the number of required groups modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3
2 3 3

```




```input2
4
0 1 2 3

```




```input3
6
5 2 0 5 2 1

```




```output1
0

```




```output2
10

```




```output3
53

```


