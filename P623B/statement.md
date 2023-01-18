## Description

<div><p>You are given array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>n</i></span>. You may consecutively apply two operations to this array:</p><ul> <li> remove some subsegment (continuous subsequence) of length <span class="tex-span"><i>m</i> &lt; <i>n</i></span> and pay for it <span class="tex-span"><i>m</i>·<i>a</i></span> coins; </li><li> change some elements of the array by at most <span class="tex-span">1</span>, and pay <span class="tex-span"><i>b</i></span> coins for each change. </li></ul><p>Please note that each of operations may be applied at most once (and may be not applied at all) so you can remove only one segment and each number may be changed (increased or decreased) by at most <span class="tex-span">1</span>. Also note, that you are not allowed to delete the whole array.</p><p>Your goal is to calculate the minimum number of coins that you need to spend in order to make the greatest common divisor of the elements of the resulting array be greater than <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000, 0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the array, the cost of removing a single element in the first operation and the cost of changing an element, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the minimum cost of changes needed to obtain an array, such that the greatest common divisor of all its elements is greater than <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000, 0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the array, the cost of removing a single element in the first operation and the cost of changing an element, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array.</p>

## Output

<p>Print a single number&nbsp;— the minimum cost of changes needed to obtain an array, such that the greatest common divisor of all its elements is greater than <span class="tex-span">1</span>.</p>





```input1
3 1 4
4 2 3

```




```input2
5 3 2
5 17 13 5 6

```




```input3
8 3 4
3 7 5 4 3 12 9 4

```




```output1
1

```




```output2
8

```




```output3
13

```



## Note

<p>In the first sample the optimal way is to remove number <span class="tex-span">3</span> and pay <span class="tex-span">1</span> coin for it.</p><p>In the second sample you need to remove a segment <span class="tex-span">[17, 13]</span> and then decrease number <span class="tex-span">6</span>. The cost of these changes is equal to <span class="tex-span">2·3 + 2 = 8</span> coins.</p>
