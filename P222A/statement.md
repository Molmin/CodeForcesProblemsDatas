## Description

<div><p>One day shooshuns found a sequence of <span class="tex-span"><i>n</i></span> integers, written on a blackboard. The shooshuns can perform one operation with it, the operation consists of two steps:</p><ol> <li> Find the number that goes <span class="tex-span"><i>k</i></span>-th in the current sequence and add the same number to the end of the sequence; </li><li> Delete the first number of the current sequence. </li></ol><p>The shooshuns wonder after how many operations all numbers on the board will be the same and whether all numbers will ever be the same.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the sequence that the shooshuns found.</p></div><div class="output-specification"><p>Print the minimum number of operations, required for all numbers on the blackboard to become the same. If it is impossible to achieve, print -1.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the sequence that the shooshuns found.</p>

## Output

<p>Print the minimum number of operations, required for all numbers on the blackboard to become the same. If it is impossible to achieve, print -1.</p>





```input1
3 2
3 1 1

```




```input2
3 1
3 1 1

```




```output1
1

```




```output2
-1

```



## Note

<p>In the first test case after the first operation the blackboard will have sequence <span class="tex-font-style-tt">[1, 1, 1]</span>. So, one operation is enough to make all numbers the same. Thus, the answer equals one.</p><p>In the second test case the sequence will never consist of the same numbers. It will always contain at least two distinct numbers 3 and 1. Thus, the answer equals -1.</p>
