## Description

<div><p>The Little Elephant enjoys recursive functions.</p><p>This time he enjoys the sorting function. Let <span class="tex-span"><i>a</i></span> is a permutation of an integers from 1 to <span class="tex-span"><i>n</i></span>, inclusive, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th element of the permutation. The Little Elephant's recursive function <span class="tex-span"><i>f</i>(<i>x</i>)</span>, that sorts the first <span class="tex-span"><i>x</i></span> permutation's elements, works as follows:</p><ul> <li> If <span class="tex-span"><i>x</i> = 1</span>, exit the function. </li><li> Otherwise, call <span class="tex-span"><i>f</i>(<i>x</i> - 1)</span>, and then make <span class="tex-span"><i>swap</i>(<i>a</i><sub class="lower-index"><i>x</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>x</i></sub>)</span> (swap the <span class="tex-span"><i>x</i></span>-th and <span class="tex-span">(<i>x</i> - 1)</span>-th elements of <span class="tex-span"><i>a</i></span>). </li></ul><p>The Little Elephant's teacher believes that this function does not work correctly. But that-be do not get an F, the Little Elephant wants to show the performance of its function. Help him, find a permutation of numbers from 1 to <span class="tex-span"><i>n</i></span>, such that after performing the Little Elephant's function (that is call <span class="tex-span"><i>f</i>(<i>n</i>)</span>), the permutation will be sorted in ascending order.</p></div><div class="input-specification"><p>A single line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the size of permutation.</p></div><div class="output-specification"><p>In a single line print <span class="tex-span"><i>n</i></span> distinct integers from 1 to <span class="tex-span"><i>n</i></span> — the required permutation. Numbers in a line should be separated by spaces.</p><p>It is guaranteed that the answer exists.</p></div>

## Input

<p>A single line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the size of permutation.</p>

## Output

<p>In a single line print <span class="tex-span"><i>n</i></span> distinct integers from 1 to <span class="tex-span"><i>n</i></span> — the required permutation. Numbers in a line should be separated by spaces.</p><p>It is guaranteed that the answer exists.</p>





```input1
1

```




```input2
2

```




```output1
1
```




```output2
2 1
```


