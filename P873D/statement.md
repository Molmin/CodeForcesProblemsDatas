## Description

<div><p>Merge sort is a well-known sorting algorithm. The main function that sorts the elements of array <span class="tex-span"><i>a</i></span> with indices from <span class="tex-span">[<i>l</i>, <i>r</i>)</span> can be implemented as follows:</p><ol> <li> If the segment <span class="tex-span">[<i>l</i>, <i>r</i>)</span> is already sorted in non-descending order (that is, for any <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> &lt; <i>r</i> - 1</span> <span class="tex-span"><i>a</i>[<i>i</i>] ≤ <i>a</i>[<i>i</i> + 1]</span>), then end the function call; </li><li> Let <img align="middle" class="tex-formula" src="file://bvuHcme1.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> Call <span class="tex-span"><i>mergesort</i>(<i>a</i>, <i>l</i>, <i>mid</i>)</span>; </li><li> Call <span class="tex-span"><i>mergesort</i>(<i>a</i>, <i>mid</i>, <i>r</i>)</span>; </li><li> Merge segments <span class="tex-span">[<i>l</i>, <i>mid</i>)</span> and <span class="tex-span">[<i>mid</i>, <i>r</i>)</span>, making the segment <span class="tex-span">[<i>l</i>, <i>r</i>)</span> sorted in non-descending order. The merge algorithm doesn't call any other functions. </li></ol><p>The array in this problem is <span class="tex-span">0</span>-indexed, so to sort the whole array, you need to call <span class="tex-span"><i>mergesort</i>(<i>a</i>, 0, <i>n</i>)</span>.</p><p>The number of calls of function <span class="tex-span"><i>mergesort</i></span> is very important, so Ivan has decided to calculate it while sorting the array. For example, if <span class="tex-span"><i>a</i> = {1, 2, 3, 4}</span>, then there will be <span class="tex-span">1</span> call of <span class="tex-span"><i>mergesort</i></span> — <span class="tex-span"><i>mergesort</i>(0, 4)</span>, which will check that the array is sorted and then end. If <span class="tex-span"><i>a</i> = {2, 1, 3}</span>, then the number of calls is <span class="tex-span">3</span>: first of all, you call <span class="tex-span"><i>mergesort</i>(0, 3)</span>, which then sets <span class="tex-span"><i>mid</i> = 1</span> and calls <span class="tex-span"><i>mergesort</i>(0, 1)</span> and <span class="tex-span"><i>mergesort</i>(1, 3)</span>, which do not perform any recursive calls because segments <span class="tex-span">(0, 1)</span> and <span class="tex-span">(1, 3)</span> are sorted.</p><p>Ivan has implemented the program that counts the number of <span class="tex-span"><i>mergesort</i></span> calls, but now he needs to test it. To do this, he needs to find an array <span class="tex-span"><i>a</i></span> such that <span class="tex-span"><i>a</i></span> is a permutation of size <span class="tex-span"><i>n</i></span> (that is, the number of elements in <span class="tex-span"><i>a</i></span> is <span class="tex-span"><i>n</i></span>, and every integer number from <span class="tex-span">[1, <i>n</i>]</span> can be found in this array), and the number of <span class="tex-span"><i>mergesort</i></span> calls when sorting the array is exactly <span class="tex-span"><i>k</i></span>.</p><p>Help Ivan to find an array he wants!</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 200000</span>) — the size of a desired permutation and the number of <span class="tex-span"><i>mergesort</i></span> calls required to sort it.</p></div><div class="output-specification"><p>If a permutation of size <span class="tex-span"><i>n</i></span> such that there will be exactly <span class="tex-span"><i>k</i></span> calls of <span class="tex-span"><i>mergesort</i></span> while sorting it doesn't exist, output <span class="tex-span"> - 1</span>. Otherwise output <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i>[0], <i>a</i>[1], ..., <i>a</i>[<i>n</i> - 1]</span> — the elements of a permutation that would meet the required conditions. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 200000</span>) — the size of a desired permutation and the number of <span class="tex-span"><i>mergesort</i></span> calls required to sort it.</p>

## Output

<p>If a permutation of size <span class="tex-span"><i>n</i></span> such that there will be exactly <span class="tex-span"><i>k</i></span> calls of <span class="tex-span"><i>mergesort</i></span> while sorting it doesn't exist, output <span class="tex-span"> - 1</span>. Otherwise output <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i>[0], <i>a</i>[1], ..., <i>a</i>[<i>n</i> - 1]</span> — the elements of a permutation that would meet the required conditions. If there are multiple answers, print any of them.</p>





```input1
3 3

```




```input2
4 1

```




```input3
5 6

```




```output1
2 1 3
```




```output2
1 2 3 4
```




```output3
-1

```


