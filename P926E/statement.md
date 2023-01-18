## Description

<div><p>You are given a sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>While possible, you perform the following operation: find a pair of equal consecutive elements. If there are more than one such pair, find the leftmost (with the smallest indices of elements). If the two integers are equal to <span class="tex-span"><i>x</i></span>, delete both and insert a single integer <span class="tex-span"><i>x</i> + 1</span> on their place. This way the number of elements in the sequence is decreased by <span class="tex-span">1</span> on each step. </p><p>You stop performing the operation when there is no pair of equal consecutive elements.</p><p>For example, if the initial sequence is <span class="tex-span">[5, 2, 1, 1, 2, 2]</span>, then after the first operation you get <span class="tex-span">[5, 2, 2, 2, 2]</span>, after the second — <span class="tex-span">[5, 3, 2, 2]</span>, after the third — <span class="tex-span">[5, 3, 3]</span>, and finally after the fourth you get <span class="tex-span">[5, 4]</span>. After that there are no equal consecutive elements left in the sequence, so you stop the process.</p><p>Determine the final sequence after you stop performing the operation.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in the sequence.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span> — the number of elements in the sequence after you stop performing the operation. </p><p>In the second line print <span class="tex-span"><i>k</i></span> integers&nbsp;— the sequence after you stop performing the operation.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in the sequence.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span> — the number of elements in the sequence after you stop performing the operation. </p><p>In the second line print <span class="tex-span"><i>k</i></span> integers&nbsp;— the sequence after you stop performing the operation.</p>





```input1
6
5 2 1 1 2 2

```




```input2
4
1000000000 1000000000 1000000000 1000000000

```




```input3
7
4 10 22 11 12 5 6

```




```output1
2
5 4
```




```output2
1
1000000002
```




```output3
7
4 10 22 11 12 5 6
```



## Note

<p>The first example is described in the statements.</p><p>In the second example the initial sequence is <span class="tex-span">[1000000000, 1000000000, 1000000000, 1000000000]</span>. After the first operation the sequence is equal to <span class="tex-span">[1000000001, 1000000000, 1000000000]</span>. After the second operation the sequence is <span class="tex-span">[1000000001, 1000000001]</span>. After the third operation the sequence is <span class="tex-span">[1000000002]</span>.</p><p>In the third example there are no two equal consecutive elements initially, so the sequence does not change.</p>
