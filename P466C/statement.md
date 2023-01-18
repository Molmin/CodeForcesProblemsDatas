## Description

<div><p>You've got array <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span>, consisting of <span class="tex-span"><i>n</i></span> integers. Count the number of ways to split all the elements of the array into three contiguous parts so that the sum of elements in each part is the same. </p><p>More formally, you need to find the number of such pairs of indices <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(2 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i> - 1)</span>, that <img align="middle" class="tex-formula" src="file://2nr5rMFB.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>, showing how many numbers are in the array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1]</span>, <span class="tex-span"><i>a</i>[2]</span>, ..., <span class="tex-span"><i>a</i>[<i>n</i>]</span> <span class="tex-span">(|<i>a</i>[<i>i</i>]| ≤  10<sup class="upper-index">9</sup>)</span> — the elements of array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the number of ways to split the array into three parts with the same sum.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>, showing how many numbers are in the array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1]</span>, <span class="tex-span"><i>a</i>[2]</span>, ..., <span class="tex-span"><i>a</i>[<i>n</i>]</span> <span class="tex-span">(|<i>a</i>[<i>i</i>]| ≤  10<sup class="upper-index">9</sup>)</span> — the elements of array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print a single integer — the number of ways to split the array into three parts with the same sum.</p>





```input1
5
1 2 3 0 3

```




```input2
4
0 1 -1 0

```




```input3
2
4 1

```




```output1
2

```




```output2
1

```




```output3
0

```


