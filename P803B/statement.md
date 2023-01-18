## Description

<div><p>You are given the array of integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>. For each element find the distance to the nearest zero (to the element which equals to zero). There is at least one zero element in the given array.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — length of the array <span class="tex-span"><i>a</i></span>. The second line contains integer elements of the array separated by single spaces (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the sequence <span class="tex-span"><i>d</i><sub class="lower-index">0</sub>, <i>d</i><sub class="lower-index">1</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the difference of indices between <span class="tex-span"><i>i</i></span> and nearest <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = 0</span>. It is possible that <span class="tex-span"><i>i</i> = <i>j</i></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — length of the array <span class="tex-span"><i>a</i></span>. The second line contains integer elements of the array separated by single spaces (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the sequence <span class="tex-span"><i>d</i><sub class="lower-index">0</sub>, <i>d</i><sub class="lower-index">1</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the difference of indices between <span class="tex-span"><i>i</i></span> and nearest <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = 0</span>. It is possible that <span class="tex-span"><i>i</i> = <i>j</i></span>.</p>





```input1
9
2 1 0 3 0 0 3 2 4

```




```input2
5
0 1 2 3 4

```




```input3
7
5 6 0 1 -2 3 4

```




```output1
2 1 0 1 0 0 1 2 3
```




```output2
0 1 2 3 4
```




```output3
2 1 0 1 2 3 4
```


