## Description

<div><p>Jeff's friends know full well that the boy likes to get sequences and arrays for his birthday. Thus, Jeff got sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> for his birthday.</p><p>Jeff hates inversions in sequences. An inversion in sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is a pair of indexes <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i>)</span>, such that an inequality <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i></sub></span> holds.</p><p>Jeff can multiply some numbers of the sequence <span class="tex-span"><i>p</i></span> by -1. At that, he wants the number of inversions in the sequence to be minimum. Help Jeff and find the minimum number of inversions he manages to get.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers — sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>p</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup>)</span>. The numbers are separated by spaces.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the minimum number of inversions Jeff can get.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers — sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>p</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup>)</span>. The numbers are separated by spaces.</p>

## Output

<p>In a single line print the answer to the problem — the minimum number of inversions Jeff can get.</p>





```input1
2
2 1

```




```input2
9
-2 0 -1 0 -1 2 1 0 -1

```




```output1
0

```




```output2
6

```


