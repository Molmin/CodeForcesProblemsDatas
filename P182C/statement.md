## Description

<div><p>And here goes another problem on arrays. You are given positive integer <span class="tex-span"><i>len</i></span> and array <span class="tex-span"><i>a</i></span> which consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. Let's introduce two characteristics for the given array.</p><ul> <li> Let's consider an arbitrary interval of the array with length <span class="tex-span"><i>len</i></span>, starting in position <span class="tex-span"><i>i</i></span>. Value <img align="middle" class="tex-formula" src="file://riVjWJCX.png" style="max-width: 100.0%;max-height: 100.0%;">, is the <span class="tex-font-style-bf">modular sum</span> on the chosen interval. In other words, the modular sum is the sum of integers on the chosen interval with length <span class="tex-span"><i>len</i></span>, taken in its absolute value.</li><li> Value <img align="middle" class="tex-formula" src="file://YOjEucYd.png" style="max-width: 100.0%;max-height: 100.0%;"> is the <span class="tex-font-style-bf">optimal sum</span> of the array. In other words, the optimal sum of an array is the maximum of all modular sums on various intervals of array with length <span class="tex-span"><i>len</i></span>. </li></ul><p>Your task is to calculate the optimal sum of the given array <span class="tex-span"><i>a</i></span>. However, before you do the calculations, you are allowed to produce <span class="tex-font-style-bf">no more</span> than <span class="tex-span"><i>k</i></span> consecutive operations of the following form with this array: one operation means taking an arbitrary number from array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and multiply it by -1. In other words, no more than <span class="tex-span"><i>k</i></span> times you are allowed to take an arbitrary number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from the array and replace it with <span class="tex-span"> - <i>a</i><sub class="lower-index"><i>i</i></sub></span>. Each number of the array is allowed to choose an arbitrary number of times.</p><p>Your task is to calculate the maximum possible optimal sum of the array after at most <span class="tex-span"><i>k</i></span> operations described above are completed.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>len</i></span> (<span class="tex-span">1 ≤ <i>len</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the array and the length of the chosen subinterval of the array, correspondingly. </p><p>The second line contains a sequence consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the original array. </p><p>The third line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the maximum allowed number of operations. </p><p>All numbers in lines are separated by a single space.</p></div><div class="output-specification"><p>In a single line print the maximum possible optimal sum after no more than <span class="tex-span"><i>k</i></span> acceptable operations are fulfilled. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>len</i></span> (<span class="tex-span">1 ≤ <i>len</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the array and the length of the chosen subinterval of the array, correspondingly. </p><p>The second line contains a sequence consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the original array. </p><p>The third line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the maximum allowed number of operations. </p><p>All numbers in lines are separated by a single space.</p>

## Output

<p>In a single line print the maximum possible optimal sum after no more than <span class="tex-span"><i>k</i></span> acceptable operations are fulfilled. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 3
0 -2 3 -5 1
2

```




```input2
5 2
1 -3 -10 4 1
3

```




```input3
3 3
-2 -5 4
1

```




```output1
10

```




```output2
14

```




```output3
11

```


