## Description

<div><p>You are given three sticks with positive integer lengths of <span class="tex-span"><i>a</i>, <i>b</i></span>, and <span class="tex-span"><i>c</i></span> centimeters. You can increase length of some of them by some positive integer number of centimeters (different sticks can be increased by a different length), but in total by at most <span class="tex-span"><i>l</i></span> centimeters. In particular, it is allowed not to increase the length of any stick.</p><p>Determine the number of ways to increase the lengths of some sticks so that you can form from them a non-degenerate (that is, having a positive area) triangle. Two ways are considered different, if the length of some stick is increased by different number of centimeters in them.</p></div><div class="input-specification"><p>The single line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>l</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>l</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print a single integer — the number of ways to increase the sizes of the sticks by the total of at most <span class="tex-span"><i>l</i></span> centimeters, so that you can make a non-degenerate triangle from it.</p></div>

## Input

<p>The single line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>l</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>l</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print a single integer — the number of ways to increase the sizes of the sticks by the total of at most <span class="tex-span"><i>l</i></span> centimeters, so that you can make a non-degenerate triangle from it.</p>





```input1
1 1 1 2

```




```input2
1 2 3 1

```




```input3
10 2 1 7

```




```output1
4

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample test you can either not increase any stick or increase any two sticks by <span class="tex-span">1</span> centimeter.</p><p>In the second sample test you can increase either the first or the second stick by one centimeter. Note that the triangle made from the initial sticks is degenerate and thus, doesn't meet the conditions.</p>
