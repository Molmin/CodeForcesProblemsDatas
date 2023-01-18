## Description

<div><p>Vasya has an array of integers of length <span class="tex-span"><i>n</i></span>.</p><p>Vasya performs the following operations on the array: on each step he finds the longest segment of consecutive equal integers (the leftmost, if there are several such segments) and removes it. For example, if Vasya's array is <span class="tex-span">[13, 13, 7, 7, 7, 2, 2, 2]</span>, then after one operation it becomes <span class="tex-span">[13, 13, 2, 2, 2]</span>.</p><p>Compute the number of operations Vasya should make until the array becomes empty, i.e. Vasya removes all elements from it.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the length of the array.</p><p>The second line contains a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — Vasya's array.</p></div><div class="output-specification"><p>Print the number of operations Vasya should make to remove all elements from the array.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the length of the array.</p><p>The second line contains a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — Vasya's array.</p>

## Output

<p>Print the number of operations Vasya should make to remove all elements from the array.</p>





```input1
4
2 5 5 2

```




```input2
5
6 3 4 1 5

```




```input3
8
4 4 4 2 2 100 100 100

```




```input4
6
10 10 50 10 50 50

```




```output1
2

```




```output2
5

```




```output3
3

```




```output4
4

```



## Note

<p>In the first example, at first Vasya removes two fives at the second and third positions. The array becomes <span class="tex-span">[2, 2]</span>. In the second operation Vasya removes two twos at the first and second positions. After that the array becomes empty.</p><p>In the second example Vasya has to perform five operations to make the array empty. In each of them he removes the first element from the array.</p><p>In the third example Vasya needs three operations. In the first operation he removes all integers <span class="tex-span">4</span>, in the second — all integers <span class="tex-span">100</span>, in the third — all integers <span class="tex-span">2</span>.</p><p>In the fourth example in the first operation Vasya removes the first two integers <span class="tex-span">10</span>. After that the array becomes <span class="tex-span">[50, 10, 50, 50]</span>. Then in the second operation Vasya removes the two rightmost integers <span class="tex-span">50</span>, so that the array becomes <span class="tex-span">[50, 10]</span>. In the third operation he removes the remaining <span class="tex-span">50</span>, and the array becomes <span class="tex-span">[10]</span> after that. In the last, fourth operation he removes the only remaining <span class="tex-span">10</span>. The array is empty after that.</p>
