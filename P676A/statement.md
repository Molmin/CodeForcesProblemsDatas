## Description

<div><p>Nicholas has an array <span class="tex-span"><i>a</i></span> that contains <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct</span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. In other words, Nicholas has a permutation of size <span class="tex-span"><i>n</i></span>.</p><p>Nicholas want the minimum element (integer <span class="tex-span">1</span>) and the maximum element (integer <span class="tex-span"><i>n</i></span>) to be as far as possible from each other. He wants to perform exactly one swap in order to maximize the distance between the minimum and the maximum elements. The distance between two elements is considered to be equal to the absolute difference between their positions.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the size of the permutation.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the element at the <span class="tex-span"><i>i</i></span>-th position.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible distance between the minimum and the maximum elements Nicholas can achieve by performing exactly one swap.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the size of the permutation.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the element at the <span class="tex-span"><i>i</i></span>-th position.</p>

## Output

<p>Print a single integer&nbsp;— the maximum possible distance between the minimum and the maximum elements Nicholas can achieve by performing exactly one swap.</p>





```input1
5
4 5 1 3 2

```




```input2
7
1 6 5 3 4 7 2

```




```input3
6
6 5 4 3 2 1

```




```output1
3

```




```output2
6

```




```output3
5

```



## Note

<p>In the first sample, one may obtain the optimal answer by swapping elements <span class="tex-span">1</span> and <span class="tex-span">2</span>.</p><p>In the second sample, the minimum and the maximum elements will be located in the opposite ends of the array if we swap <span class="tex-span">7</span> and <span class="tex-span">2</span>.</p><p>In the third sample, the distance between the minimum and the maximum elements is already maximum possible, so we just perform some unnecessary swap, for example, one can swap <span class="tex-span">5</span> and <span class="tex-span">2</span>.</p>
