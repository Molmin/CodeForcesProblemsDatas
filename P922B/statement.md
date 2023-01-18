## Description

<div><p>Imp is in a magic forest, where xorangles grow (wut?)</p><center> <img class="tex-graphics" src="file://AXq7ciGz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A xorangle of order <span class="tex-span"><i>n</i></span> is such a non-degenerate triangle, that lengths of its sides are integers not exceeding <span class="tex-span"><i>n</i></span>, and the xor-sum of the lengths is equal to zero. Imp has to count the number of distinct xorangles of order <span class="tex-span"><i>n</i></span> to get out of the forest. </p><p>Formally, for a given integer <span class="tex-span"><i>n</i></span> you have to find the number of such triples <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span>, that:</p><ul> <li> <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>c</i> ≤ <i>n</i></span>; </li><li> <img align="middle" class="tex-formula" src="file://GJjNkUlw.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://BS52Mi3J.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise xor</a> of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. </li><li> <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> form a non-degenerate (with strictly positive area) triangle. </li></ul></div><div class="input-specification"><p>The only line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2500)</span>.</p></div><div class="output-specification"><p>Print the number of xorangles of order <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The only line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2500)</span>.</p>

## Output

<p>Print the number of xorangles of order <span class="tex-span"><i>n</i></span>.</p>





```input1
6

```




```input2
10

```




```output1
1

```




```output2
2

```



## Note

<p>The only xorangle in the first sample is <span class="tex-span">(3, 5, 6)</span>.</p>
