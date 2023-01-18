## Description

<div><p>The Little Elephant loves sortings.</p><p>He has an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. Let's number the array elements from 1 to <span class="tex-span"><i>n</i></span>, then the <span class="tex-span"><i>i</i></span>-th element will be denoted as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The Little Elephant can make one move to choose an arbitrary pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span> and increase <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span">1</span> for all <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>.</p><p>Help the Little Elephant find the minimum number of moves he needs to convert array <span class="tex-span"><i>a</i></span> to an arbitrary array sorted in the non-decreasing order. Array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> elements, is sorted in the non-decreasing order if for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> holds.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span>. The next line contains <span class="tex-span"><i>n</i></span> integers, separated by single spaces — array <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The array elements are listed in the line in the order of their index's increasing.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span>. The next line contains <span class="tex-span"><i>n</i></span> integers, separated by single spaces — array <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The array elements are listed in the line in the order of their index's increasing.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
1 2 3

```




```input2
3
3 2 1

```




```input3
4
7 4 1 47

```




```output1
0

```




```output2
2

```




```output3
6

```



## Note

<p>In the first sample the array is already sorted in the non-decreasing order, so the answer is <span class="tex-span">0</span>.</p><p>In the second sample you need to perform two operations: first increase numbers from second to third (after that the array will be: <span class="tex-font-style-tt">[3, 3, 2]</span>), and second increase only the last element (the array will be: <span class="tex-font-style-tt">[3, 3, 3]</span>).</p><p>In the third sample you should make at least 6 steps. The possible sequence of the operations is: <span class="tex-font-style-tt">(2; 3), (2; 3), (2; 3), (3; 3), (3; 3), (3; 3)</span>. After that the array converts to <span class="tex-font-style-tt">[7, 7, 7, 47]</span>.</p>
