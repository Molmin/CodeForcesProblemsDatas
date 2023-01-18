## Description

<div><p>You've got array <span class="tex-span"><i>A</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers and a positive integer <span class="tex-span"><i>k</i></span>. Array <span class="tex-span"><i>A</i></span> is indexed by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>You need to permute the array elements so that value </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://ffD1g6A5.png" style="max-width: 100.0%;max-height: 100.0%;"></center> became minimal possible. In particular, it is allowed not to change order of elements at all.</div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(5000, <i>n</i> - 1)</span>). </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>A</i>[1], <i>A</i>[2], ..., <i>A</i>[<i>n</i>]</span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>A</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>), separate by spaces — elements of the array <span class="tex-span"><i>A</i></span>.</p></div><div class="output-specification"><p>Print the minimum possible value of the sum described in the statement.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(5000, <i>n</i> - 1)</span>). </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>A</i>[1], <i>A</i>[2], ..., <i>A</i>[<i>n</i>]</span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>A</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>), separate by spaces — elements of the array <span class="tex-span"><i>A</i></span>.</p>

## Output

<p>Print the minimum possible value of the sum described in the statement.</p>





```input1
3 2
1 2 4

```




```input2
5 2
3 -5 3 -5 3

```




```input3
6 3
4 3 4 3 2 5

```




```output1
1

```




```output2
0

```




```output3
3

```



## Note

<p>In the first test one of the optimal permutations is <span class="tex-span">1&nbsp;4&nbsp;2</span>. </p><p>In the second test the initial order is optimal. </p><p>In the third test one of the optimal permutations is <span class="tex-span">2&nbsp;3&nbsp;4&nbsp;4&nbsp;3&nbsp;5</span>.</p>
