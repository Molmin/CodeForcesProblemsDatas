## Description

<div><p>"Hey, it's homework time" — thought Polycarpus and of course he started with his favourite subject, IT. Polycarpus managed to solve all tasks but for the last one in 20 minutes. However, as he failed to solve the last task after some considerable time, the boy asked you to help him.</p><p>The sequence of <span class="tex-span"><i>n</i></span> integers is called a permutation if it contains all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> exactly once.</p><p>You are given an arbitrary sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> containing <span class="tex-span"><i>n</i></span> integers. Each integer is not less than <span class="tex-span">1</span> and not greater than <span class="tex-span">5000</span>. Determine what minimum number of elements Polycarpus needs to change to get a permutation (he should not delete or add numbers). In a single change he can modify any single sequence element (i. e. replace it with another integer).</p></div><div class="input-specification"><p>The first line of the input data contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) which represents how many numbers are in the sequence. The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000, 1 ≤ <i>i</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the only number — the minimum number of changes needed to get the permutation.</p></div>

## Input

<p>The first line of the input data contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) which represents how many numbers are in the sequence. The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000, 1 ≤ <i>i</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print the only number — the minimum number of changes needed to get the permutation.</p>





```input1
3
3 1 2

```




```input2
2
2 2

```




```input3
5
5 3 3 3 1

```




```output1
0

```




```output2
1

```




```output3
2

```



## Note

<p>The first sample contains the permutation, which is why no replacements are required.</p><p>In the second sample it is enough to replace the first element with the number 1 and that will make the sequence the needed permutation.</p><p>In the third sample we can replace the second element with number 4 and the fourth element with number 2.</p>
