## Description

<div><p>This task will exclusively concentrate only on the arrays where all elements equal 1 and/or 2.</p><p>Array <span class="tex-span"><i>a</i></span> is <span class="tex-span"><i>k</i></span>-period if its length is divisible by <span class="tex-span"><i>k</i></span> and there is such array <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>k</i></span>, that <span class="tex-span"><i>a</i></span> is represented by array <span class="tex-span"><i>b</i></span> written exactly <img align="middle" class="tex-formula" src="file://VNfU2DJI.png" style="max-width: 100.0%;max-height: 100.0%;"> times consecutively. In other words, array <span class="tex-span"><i>a</i></span> is <span class="tex-span"><i>k</i></span>-periodic, if it has period of length <span class="tex-span"><i>k</i></span>.</p><p>For example, any array is <span class="tex-span"><i>n</i></span>-periodic, where <span class="tex-span"><i>n</i></span> is the array length. Array <span class="tex-span">[2, 1, 2, 1, 2, 1]</span> is at the same time 2-periodic and 6-periodic and array <span class="tex-span">[1, 2, 1, 1, 2, 1, 1, 2, 1]</span> is at the same time 3-periodic and 9-periodic.</p><p>For the given array <span class="tex-span"><i>a</i></span>, consisting only of numbers one and two, find the minimum number of elements to change to make the array <span class="tex-span"><i>k</i></span>-periodic. If the array already is <span class="tex-span"><i>k</i></span>-periodic, then the required value equals <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line of the input contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span>, where <span class="tex-span"><i>n</i></span> is the length of the array and the value <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>. The second line contains the sequence of elements of the given array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the array.</p></div><div class="output-specification"><p>Print the minimum number of array elements we need to change to make the array <span class="tex-span"><i>k</i></span>-periodic. If the array already is <span class="tex-span"><i>k</i></span>-periodic, then print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line of the input contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span>, where <span class="tex-span"><i>n</i></span> is the length of the array and the value <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>. The second line contains the sequence of elements of the given array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the array.</p>

## Output

<p>Print the minimum number of array elements we need to change to make the array <span class="tex-span"><i>k</i></span>-periodic. If the array already is <span class="tex-span"><i>k</i></span>-periodic, then print <span class="tex-font-style-tt">0</span>.</p>





```input1
6 2
2 1 2 2 2 1

```




```input2
8 4
1 1 2 1 1 1 2 1

```




```input3
9 3
2 1 1 1 2 1 1 1 2

```




```output1
1

```




```output2
0

```




```output3
3

```



## Note

<p>In the first sample it is enough to change the fourth element from <span class="tex-font-style-tt">2</span> to <span class="tex-font-style-tt">1</span>, then the array changes to <span class="tex-span">[2, 1, 2, 1, 2, 1]</span>.</p><p>In the second sample, the given array already is 4-periodic.</p><p>In the third sample it is enough to replace each occurrence of number two by number one. In this case the array will look as <span class="tex-span">[1, 1, 1, 1, 1, 1, 1, 1, 1]</span> — this array is simultaneously 1-, 3- and 9-periodic.</p>
