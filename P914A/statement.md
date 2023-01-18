## Description

<div><p>Given an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of <span class="tex-span"><i>n</i></span> integers, find the largest number in the array that is not a perfect square.</p><p>A number <span class="tex-span"><i>x</i></span> is said to be a perfect square if there exists an integer <span class="tex-span"><i>y</i></span> such that <span class="tex-span"><i>x</i> = <i>y</i><sup class="upper-index">2</sup></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the elements of the array.</p><p>It is guaranteed that at least one element of the array is not a perfect square.</p></div><div class="output-specification"><p>Print the largest number in the array which is not a perfect square. It is guaranteed that an answer always exists.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the elements of the array.</p><p>It is guaranteed that at least one element of the array is not a perfect square.</p>

## Output

<p>Print the largest number in the array which is not a perfect square. It is guaranteed that an answer always exists.</p>





```input1
2
4 2

```




```input2
8
1 2 4 8 16 32 64 576

```




```output1
2

```




```output2
32

```



## Note

<p>In the first sample case, <span class="tex-span">4</span> is a perfect square, so the largest number in the array that is not a perfect square is <span class="tex-span">2</span>.</p>
