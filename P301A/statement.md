## Description

<div><p>Yaroslav has an array, consisting of <span class="tex-span">(2·<i>n</i> - 1)</span> integers. In a single operation Yaroslav can change the sign of exactly <span class="tex-span"><i>n</i></span> elements in the array. In other words, in one operation Yaroslav can select exactly <span class="tex-span"><i>n</i></span> array elements, and multiply each of them by -1.</p><p>Yaroslav is now wondering: what maximum sum of array elements can be obtained if it is allowed to perform any number of described operations?</p><p>Help Yaroslav.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 100)</span>. The second line contains <span class="tex-span">(2·<i>n</i> - 1)</span> integers — the array elements. The array elements do not exceed <span class="tex-span">1000</span> in their absolute value.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the maximum sum that Yaroslav can get.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 100)</span>. The second line contains <span class="tex-span">(2·<i>n</i> - 1)</span> integers — the array elements. The array elements do not exceed <span class="tex-span">1000</span> in their absolute value.</p>

## Output

<p>In a single line print the answer to the problem — the maximum sum that Yaroslav can get.</p>





```input1
2
50 50 50

```




```input2
2
-1 -100 -1

```




```output1
150

```




```output2
100

```



## Note

<p>In the first sample you do not need to change anything. The sum of elements equals <span class="tex-span">150</span>.</p><p>In the second sample you need to change the sign of the first two elements. Then we get the sum of the elements equal to <span class="tex-span">100</span>.</p>
