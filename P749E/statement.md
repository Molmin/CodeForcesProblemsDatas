## Description

<div><p>You are given a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Exactly once you apply the following operation to this permutation: pick a random segment and shuffle its elements. Formally:</p><ol> <li> Pick a random segment (continuous subsequence) from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>. All <img align="middle" class="tex-formula" src="file://9RPFGHLu.png" style="max-width: 100.0%;max-height: 100.0%;"> segments are equiprobable. </li><li> Let <span class="tex-span"><i>k</i> = <i>r</i> - <i>l</i> + 1</span>, i.e. the length of the chosen segment. Pick a random permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span>. All <span class="tex-span"><i>k</i>!</span> permutation are equiprobable. </li><li> This permutation is applied to elements of the chosen segment, i.e. permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>l</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>r</i></sub>, <i>a</i><sub class="lower-index"><i>r</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is transformed to <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>l</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>l</i> - 1 + <i>p</i><sub class="lower-index">1</sub></sub>, <i>a</i><sub class="lower-index"><i>l</i> - 1 + <i>p</i><sub class="lower-index">2</sub></sub>, ..., <i>a</i><sub class="lower-index"><i>l</i> - 1 + <i>p</i><sub class="lower-index"><i>k</i> - 1</sub></sub>, <i>a</i><sub class="lower-index"><i>l</i> - 1 + <i>p</i><sub class="lower-index"><i>k</i></sub></sub>, <i>a</i><sub class="lower-index"><i>r</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </li></ol><p><span class="tex-font-style-underline">Inversion</span> if a pair of elements (not necessary neighbouring) with the wrong relative order. In other words, the number of inversion is equal to the number of pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>. Find the expected number of inversions after we apply exactly one operation mentioned above.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>&nbsp;— elements of the permutation.</p></div><div class="output-specification"><p>Print one real value&nbsp;— the expected number of inversions. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://KgM7Aucj.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>&nbsp;— elements of the permutation.</p>

## Output

<p>Print one real value&nbsp;— the expected number of inversions. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://KgM7Aucj.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3
2 3 1

```




```output1
1.916666666666666666666666666667

```


