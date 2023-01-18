## Description

<div><p>Petya has <span class="tex-span"><i>n</i></span> integers: <span class="tex-span">1, 2, 3, ..., <i>n</i></span>. He wants to split these integers in <span class="tex-font-style-bf">two non-empty</span> groups in such a way that the absolute difference of sums of integers in each group is as small as possible. </p><p>Help Petya to split the integers. Each of <span class="tex-span"><i>n</i></span> integers should be exactly in one group.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 60 000</span>) — the number of integers Petya has.</p></div><div class="output-specification"><p>Print the smallest possible absolute difference in the first line.</p><p>In the second line print the size of the first group, followed by the integers in that group. You can print these integers in arbitrary order. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 60 000</span>) — the number of integers Petya has.</p>

## Output

<p>Print the smallest possible absolute difference in the first line.</p><p>In the second line print the size of the first group, followed by the integers in that group. You can print these integers in arbitrary order. If there are multiple answers, print any of them.</p>





```input1
4

```




```input2
2

```




```output1
0
2 1 4 

```




```output2
1
1 1 

```



## Note

<p>In the first example you have to put integers <span class="tex-span">1</span> and <span class="tex-span">4</span> in the first group, and <span class="tex-span">2</span> and <span class="tex-span">3</span> in the second. This way the sum in each group is <span class="tex-span">5</span>, and the absolute difference is <span class="tex-span">0</span>.</p><p>In the second example there are only two integers, and since both groups should be non-empty, you have to put one integer in the first group and one in the second. This way the absolute difference of sums of integers in each group is <span class="tex-span">1</span>.</p>
