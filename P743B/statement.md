## Description

<div><p>Chloe, the same as Vladik, is a competitive programmer. She didn't have any problems to get to the olympiad like Vladik, but she was confused by the task proposed on the olympiad.</p><p>Let's consider the following algorithm of generating a sequence of integers. Initially we have a sequence consisting of a single element equal to <span class="tex-span">1</span>. Then we perform <span class="tex-span">(<i>n</i> - 1)</span> steps. On each step we take the sequence we've got on the previous step, append it to the end of itself and insert in the middle the minimum positive integer we haven't used before. For example, we get the sequence <span class="tex-span">[1, 2, 1]</span> after the first step, the sequence <span class="tex-span">[1, 2, 1, 3, 1, 2, 1]</span> after the second step.</p><p>The task is to find the value of the element with index <span class="tex-span"><i>k</i></span> (the elements are numbered from <span class="tex-span">1</span>) in the obtained sequence, i.&nbsp;e. after <span class="tex-span">(<i>n</i> - 1)</span> steps.</p><p>Please help Chloe to solve the problem!</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2<sup class="upper-index"><i>n</i></sup> - 1</span>).</p></div><div class="output-specification"><p>Print single integer&nbsp;— the integer at the <span class="tex-span"><i>k</i></span>-th position in the obtained sequence.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2<sup class="upper-index"><i>n</i></sup> - 1</span>).</p>

## Output

<p>Print single integer&nbsp;— the integer at the <span class="tex-span"><i>k</i></span>-th position in the obtained sequence.</p>





```input1
3 2

```




```input2
4 8

```




```output1
2
```




```output2
4
```



## Note

<p>In the first sample the obtained sequence is <span class="tex-span">[1, 2, 1, 3, 1, 2, 1]</span>. The number on the second position is <span class="tex-span">2</span>.</p><p>In the second sample the obtained sequence is <span class="tex-span">[1, 2, 1, 3, 1, 2, 1, 4, 1, 2, 1, 3, 1, 2, 1]</span>. The number on the eighth position is <span class="tex-span">4</span>.</p>
