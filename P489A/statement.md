## Description

<div><p>In this problem your goal is to sort an array consisting of <span class="tex-span"><i>n</i></span> integers in at most <span class="tex-span"><i>n</i></span> swaps. For the given array find the sequence of swaps that makes the array sorted in the non-descending order. Swaps are performed consecutively, one after another.</p><p>Note that in this problem you do not have to minimize the number of swaps — your task is to find any sequence that is no longer than <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>) — the number of array elements. The second line contains elements of array: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the array. The elements are numerated from 0 to <span class="tex-span"><i>n</i> - 1</span> from left to right. Some integers may appear in the array more than once.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of swaps. Next <span class="tex-span"><i>k</i></span> lines must contain the descriptions of the <span class="tex-span"><i>k</i></span> swaps, one per line. Each swap should be printed as a pair of integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> (<span class="tex-span">0 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i> - 1</span>), representing the swap of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>. You can print indices in the pairs in any order. The swaps are performed in the order they appear in the output, from the first to the last. It is allowed to print <span class="tex-span"><i>i</i> = <i>j</i></span> and swap the same pair of elements multiple times.</p><p>If there are multiple answers, print any of them. It is guaranteed that at least one answer exists.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>) — the number of array elements. The second line contains elements of array: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the array. The elements are numerated from 0 to <span class="tex-span"><i>n</i> - 1</span> from left to right. Some integers may appear in the array more than once.</p>

## Output

<p>In the first line print <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of swaps. Next <span class="tex-span"><i>k</i></span> lines must contain the descriptions of the <span class="tex-span"><i>k</i></span> swaps, one per line. Each swap should be printed as a pair of integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> (<span class="tex-span">0 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i> - 1</span>), representing the swap of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>. You can print indices in the pairs in any order. The swaps are performed in the order they appear in the output, from the first to the last. It is allowed to print <span class="tex-span"><i>i</i> = <i>j</i></span> and swap the same pair of elements multiple times.</p><p>If there are multiple answers, print any of them. It is guaranteed that at least one answer exists.</p>





```input1
5
5 2 5 1 4

```




```input2
6
10 20 20 40 60 60

```




```input3
2
101 100

```




```output1
2
0 3
4 2

```




```output2
0

```




```output3
1
0 1

```


