## Description

<div><p><span class="tex-font-style-it"><span class="tex-font-style-bf">Permutation</span> <span class="tex-span"><i>p</i></span> is an ordered set of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each of them doesn't exceed <span class="tex-span"><i>n</i></span>. We'll denote the <span class="tex-span"><i>i</i></span>-th element of permutation <span class="tex-span"><i>p</i></span> as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. We'll call number <span class="tex-span"><i>n</i></span> the size or the length of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</span></p><p>The decreasing coefficient of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> is the number of such <span class="tex-span"><i>i</i> (1 ≤ <i>i</i> &lt; <i>n</i>)</span>, that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &gt; <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p><p>You have numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. Your task is to print the permutation of length <span class="tex-span"><i>n</i></span> with decreasing coefficient <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The single line contains two space-separated integers: <span class="tex-span"><i>n</i>, <i>k</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> &lt; <i>n</i>)</span> — the permutation length and the decreasing coefficient.</p></div><div class="output-specification"><p>In a single line print <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the permutation of length <span class="tex-span"><i>n</i></span> with decreasing coefficient <span class="tex-span"><i>k</i></span>. </p><p>If there are several permutations that meet this condition, print any of them. It is guaranteed that the permutation with the sought parameters exists.</p></div>

## Input

<p>The single line contains two space-separated integers: <span class="tex-span"><i>n</i>, <i>k</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> &lt; <i>n</i>)</span> — the permutation length and the decreasing coefficient.</p>

## Output

<p>In a single line print <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the permutation of length <span class="tex-span"><i>n</i></span> with decreasing coefficient <span class="tex-span"><i>k</i></span>. </p><p>If there are several permutations that meet this condition, print any of them. It is guaranteed that the permutation with the sought parameters exists.</p>





```input1
5 2

```




```input2
3 0

```




```input3
3 2

```




```output1
1 5 2 4 3

```




```output2
1 2 3

```




```output3
3 2 1

```


