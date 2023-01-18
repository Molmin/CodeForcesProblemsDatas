## Description

<div><p>Sereja has <span class="tex-span"><i>m</i></span> non-empty sets of integers <span class="tex-span"><i>A</i><sub class="lower-index">1</sub>, <i>A</i><sub class="lower-index">2</sub>, ..., <i>A</i><sub class="lower-index"><i>m</i></sub></span>. What a lucky coincidence! The given sets are a partition of the set of all integers from 1 to <span class="tex-span"><i>n</i></span>. In other words, for any integer <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>v</i> ≤ <i>n</i>)</span> there is exactly one set <span class="tex-span"><i>A</i><sub class="lower-index"><i>t</i></sub></span> such that <img align="middle" class="tex-formula" src="file://YvFlKLIO.png" style="max-width: 100.0%;max-height: 100.0%;">. Also Sereja has integer <span class="tex-span"><i>d</i></span>.</p><p>Sereja decided to choose some sets from the sets he has. Let's suppose that <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>m</i>)</span> are indexes of the chosen sets. Then let's define an array of integers <span class="tex-span"><i>b</i></span>, sorted in ascending order, as a union of the chosen sets, that is, <img align="middle" class="tex-formula" src="file://Q0LSJMno.png" style="max-width: 100.0%;max-height: 100.0%;">. We'll represent the element with number <span class="tex-span"><i>j</i></span> in this array (in ascending order) as <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>. Sereja considers his choice of sets <span class="tex-font-style-it">correct</span>, if the following conditions are met:</p><center class="tex-equation"><span class="tex-span"><i>b</i><sub class="lower-index">1</sub> ≤ <i>d</i>;&nbsp;<i>b</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i>&nbsp;(1 ≤ <i>i</i> &lt; |<i>b</i>|);&nbsp;<i>n</i> - <i>d</i> + 1 ≤ <i>b</i><sub class="lower-index">|<i>b</i>|</sub>.</span></center><p>Sereja wants to know what is the minimum number of sets <span class="tex-span">(<i>k</i>)</span> that he can choose so that his choice will be correct. Help him with that.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>d</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 20)</span>. The next <span class="tex-span"><i>m</i></span> lines contain sets. The first number in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. This number denotes the size of the <span class="tex-span"><i>i</i></span>-th set. Then the line contains <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> distinct integers from 1 to <span class="tex-span"><i>n</i></span> — set <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the sets form partition of all integers from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the minimum value <span class="tex-span"><i>k</i></span> at the right choice.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>d</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 20)</span>. The next <span class="tex-span"><i>m</i></span> lines contain sets. The first number in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. This number denotes the size of the <span class="tex-span"><i>i</i></span>-th set. Then the line contains <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> distinct integers from 1 to <span class="tex-span"><i>n</i></span> — set <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the sets form partition of all integers from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>In a single line print the answer to the problem — the minimum value <span class="tex-span"><i>k</i></span> at the right choice.</p>





```input1
3 2 2
1 2
2 1 3

```




```input2
5 1 1
5 4 5 3 2 1

```




```input3
7 3 1
4 1 3 5 7
2 2 6
1 4

```




```output1
1

```




```output2
1

```




```output3
3

```


