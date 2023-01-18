## Description

<div><p><a href="https://codegolf.stackexchange.com/questions/182221/implement-the-thanos-sorting-algorithm">Thanos sort</a> is a supervillain sorting algorithm, which works as follows: if the array is not sorted, snap your fingers* to remove the first or the second half of the items, and repeat the process.</p><p>Given an input array, what is the size of the longest sorted array you can obtain from it using Thanos sort?</p><p>*Infinity Gauntlet required.</p></div><div class="input-specification"><p>The first line of input contains a single number $n$ ($1 \le n \le 16$) — the size of the array. $n$ is guaranteed to be a power of 2.</p><p>The second line of input contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 100$) — the elements of the array.</p></div><div class="output-specification"><p>Return the maximal length of a sorted array you can obtain using Thanos sort. The elements of the array have to be sorted in non-decreasing order.</p></div>

## Input

<p>The first line of input contains a single number $n$ ($1 \le n \le 16$) — the size of the array. $n$ is guaranteed to be a power of 2.</p><p>The second line of input contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 100$) — the elements of the array.</p>

## Output

<p>Return the maximal length of a sorted array you can obtain using Thanos sort. The elements of the array have to be sorted in non-decreasing order.</p>





```input1
4
1 2 2 4
```




```input2
8
11 12 1 2 13 14 3 4
```




```input3
4
7 6 5 4
```




```output1
4
```




```output2
2
```




```output3
1
```



## Note

<p>In the first example the array is already sorted, so no finger snaps are required.</p><p>In the second example the array actually has a subarray of 4 sorted elements, but you can not remove elements from different sides of the array in one finger snap. Each time you have to remove either the whole first half or the whole second half, so you'll have to snap your fingers twice to get to a 2-element sorted array.</p><p>In the third example the array is sorted in decreasing order, so you can only save one element from the ultimate destruction.</p>
