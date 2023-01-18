## Description

<div><p>You are given a permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Determine whether there's a pair of integers <span class="tex-span"><i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>;&nbsp;<i>a</i> ≠ <i>b</i>)</span> such that the element <img align="middle" class="tex-formula" src="file://m8rUnhVg.png" style="max-width: 100.0%;max-height: 100.0%;"> (note, that it is usual division, not integer one) is between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> in this permutation.</p></div><div class="input-specification"><p>First line consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300000</span>) — the size of permutation.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers — the permutation itself.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>", if such a pair exists, "<span class="tex-font-style-tt">NO</span>" otherwise (in both cases without quotes, the answer is case insensitive).</p></div>

## Input

<p>First line consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300000</span>) — the size of permutation.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers — the permutation itself.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>", if such a pair exists, "<span class="tex-font-style-tt">NO</span>" otherwise (in both cases without quotes, the answer is case insensitive).</p>





```input1
4
1 3 4 2

```




```input2
5
1 5 2 4 3

```




```output1
NO

```




```output2
YES

```



## Note

<p>In the second example <span class="tex-span">2</span> is between <span class="tex-span">1</span> and <span class="tex-span">3</span>. Additionally <span class="tex-span">4</span> is between <span class="tex-span">3</span> and <span class="tex-span">5</span>.</p>
