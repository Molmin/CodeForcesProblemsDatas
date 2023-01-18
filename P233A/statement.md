## Description

<div><p>A <span class="tex-font-style-it">permutation</span> is a sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each of them doesn't exceed <span class="tex-span"><i>n</i></span>. Let's denote the <span class="tex-span"><i>i</i></span>-th element of permutation <span class="tex-span"><i>p</i></span> as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. We'll call number <span class="tex-span"><i>n</i></span> the size of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Nickolas adores permutations. He likes some permutations more than the others. He calls such permutations perfect. A <span class="tex-font-style-it">perfect</span> permutation is such permutation <span class="tex-span"><i>p</i></span> that for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> (<span class="tex-span"><i>n</i></span> is the permutation size) the following equations hold <span class="tex-span"><i>p</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub> = <i>i</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>. Nickolas asks you to print any perfect permutation of size <span class="tex-span"><i>n</i></span> for the given <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>A single line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the permutation size.</p></div><div class="output-specification"><p>If a perfect permutation of size <span class="tex-span"><i>n</i></span> doesn't exist, print a single integer -1. Otherwise print <span class="tex-span"><i>n</i></span> distinct integers from 1 to <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — permutation <span class="tex-span"><i>p</i></span>, that is perfect. Separate printed numbers by whitespaces.</p></div>

## Input

<p>A single line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the permutation size.</p>

## Output

<p>If a perfect permutation of size <span class="tex-span"><i>n</i></span> doesn't exist, print a single integer -1. Otherwise print <span class="tex-span"><i>n</i></span> distinct integers from 1 to <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — permutation <span class="tex-span"><i>p</i></span>, that is perfect. Separate printed numbers by whitespaces.</p>





```input1
1

```




```input2
2

```




```input3
4

```




```output1
-1

```




```output2
2 1 

```




```output3
2 1 4 3 

```


