## Description

<div><p>You are given a permutation <span class="tex-span"><i>p</i></span>. Calculate the total number of inversions in all permutations that lexicographically do not exceed the given one.</p><p>As this number can be very large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the permutation. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the permutation. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2
2 1

```




```input2
3
2 1 3

```




```output1
1

```




```output2
2

```



## Note

<p>Permutation <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span> is the sequence that consists of <span class="tex-span"><i>n</i></span> distinct integers, each of them is from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>An inversion of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> is a pair of indexes <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, such that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &gt; <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Permutation <span class="tex-span"><i>a</i></span> do not exceed permutation <span class="tex-span"><i>b</i></span> lexicographically, if either <span class="tex-span"><i>a</i> = <i>b</i></span> or there exists such number <span class="tex-span"><i>i</i></span>, for which the following logical condition fulfills: <img align="middle" class="tex-formula" src="file://noUaOWZl.png" style="max-width: 100.0%;max-height: 100.0%;"> AND <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>.</p>
