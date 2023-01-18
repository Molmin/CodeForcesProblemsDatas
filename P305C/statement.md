## Description

<div><p>Ivan has got an array of <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Ivan knows that the array is sorted in the non-decreasing order. </p><p>Ivan wrote out integers <span class="tex-span">2<sup class="upper-index"><i>a</i><sub class="lower-index">1</sub></sup>, 2<sup class="upper-index"><i>a</i><sub class="lower-index">2</sub></sup>, ..., 2<sup class="upper-index"><i>a</i><sub class="lower-index"><i>n</i></sub></sup></span> on a piece of paper. Now he wonders, what minimum number of integers of form <span class="tex-span">2<sup class="upper-index"><i>b</i></sup></span> <span class="tex-span">(<i>b</i> ≥ 0)</span> need to be added to the piece of paper so that the sum of all integers written on the paper equalled <span class="tex-span">2<sup class="upper-index"><i>v</i></sup> - 1</span> for some integer <span class="tex-span"><i>v</i></span> <span class="tex-span">(<i>v</i> ≥ 0)</span>. </p><p>Help Ivan, find the required quantity of numbers.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second input line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup>)</span>. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second input line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup>)</span>. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
4
0 1 1 1

```




```input2
1
3

```




```output1
0

```




```output2
3

```



## Note

<p>In the first sample you do not need to add anything, the sum of numbers already equals <span class="tex-span">2<sup class="upper-index">3</sup> - 1 = 7</span>.</p><p>In the second sample you need to add numbers <span class="tex-span">2<sup class="upper-index">0</sup>, 2<sup class="upper-index">1</sup>, 2<sup class="upper-index">2</sup></span>.</p>
