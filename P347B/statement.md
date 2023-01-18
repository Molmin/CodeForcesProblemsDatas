## Description

<div><p>A permutation of length <span class="tex-span"><i>n</i></span> is an integer sequence such that each integer from 0 to <span class="tex-span">(<i>n</i> - 1)</span> appears exactly once in it. For example, sequence <span class="tex-span">[0, 2, 1]</span> is a permutation of length 3 while both <span class="tex-span">[0, 2, 2]</span> and <span class="tex-span">[1, 2, 3]</span> are not.</p><p>A fixed point of a function is a point that is mapped to itself by the function. A permutation can be regarded as a bijective function. We'll get a definition of a fixed point in a permutation. An integer <span class="tex-span"><i>i</i></span> is a fixed point of permutation <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> if and only if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>. For example, permutation <span class="tex-span">[0, 2, 1]</span> has <span class="tex-span">1</span> fixed point and permutation <span class="tex-span">[0, 1, 2]</span> has <span class="tex-span">3</span> fixed points.</p><p>You are given permutation <span class="tex-span"><i>a</i></span>. You are allowed to swap two elements of the permutation at most once. Your task is to maximize the number of fixed points in the resulting permutation. Note that you are allowed to make at most one swap operation.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> — the given permutation.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible number of fixed points in the permutation after at most one swap operation.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> — the given permutation.</p>

## Output

<p>Print a single integer — the maximum possible number of fixed points in the permutation after at most one swap operation.</p>





```input1
5
0 1 3 4 2

```




```output1
3

```


