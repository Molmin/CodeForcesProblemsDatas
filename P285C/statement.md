## Description

<div><p><span class="tex-font-style-it"><span class="tex-font-style-bf">Permutation</span> <span class="tex-span"><i>p</i></span> is an ordered set of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each of them doesn't exceed <span class="tex-span"><i>n</i></span>. We'll denote the <span class="tex-span"><i>i</i></span>-th element of permutation <span class="tex-span"><i>p</i></span> as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. We'll call number <span class="tex-span"><i>n</i></span> the size or the length of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</span></p><p>You have a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. In one move, you are allowed to decrease or increase any number by one. Count the minimum number of moves, needed to build a permutation from this sequence.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the size of the sought permutation. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single number — the minimum number of moves.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the size of the sought permutation. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single number — the minimum number of moves.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2
3 0

```




```input2
3
-1 -1 2

```




```output1
2

```




```output2
6

```



## Note

<p>In the first sample you should decrease the first number by one and then increase the second number by one. The resulting permutation is <span class="tex-span">(2, 1)</span>.</p><p>In the second sample you need 6 moves to build permutation <span class="tex-span">(1, 3, 2)</span>.</p>
