## Description

<div><p><span class="tex-font-style-it">Since you are the best Wraith King, Nizhniy Magazin «Mir» at the centre of Vinnytsia is offering you a discount.</span></p><p>You are given an array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span> and an integer <span class="tex-span"><i>c</i></span>. </p><p>The value of some array <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>k</i></span> is the sum of its elements except for the <img align="middle" class="tex-formula" src="file://G58hKbVx.png" style="max-width: 100.0%;max-height: 100.0%;"> smallest. For example, the value of the array <span class="tex-span">[3, 1, 6, 5, 2]</span> with <span class="tex-span"><i>c</i> = 2</span> is <span class="tex-span">3 + 6 + 5 = 14</span>.</p><p>Among all possible partitions of <span class="tex-span"><i>a</i></span> into contiguous subarrays output the smallest possible sum of the values of these subarrays.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>c</i> ≤ 100 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Output a single integer &nbsp;— the smallest possible sum of values of these subarrays of some partition of <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>c</i> ≤ 100 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Output a single integer &nbsp;— the smallest possible sum of values of these subarrays of some partition of <span class="tex-span"><i>a</i></span>.</p>





```input1
3 5
1 2 3

```




```input2
12 10
1 1 10 10 10 10 10 10 9 10 10 10

```




```input3
7 2
2 3 6 4 5 7 1

```




```input4
8 4
1 3 4 5 5 3 4 1

```




```output1
6

```




```output2
92

```




```output3
17

```




```output4
23

```



## Note

<p>In the first example any partition yields 6 as the sum.</p><p>In the second example one of the optimal partitions is <span class="tex-span">[1, 1], [10, 10, 10, 10, 10, 10, 9, 10, 10, 10]</span> with the values 2 and 90 respectively.</p><p>In the third example one of the optimal partitions is <span class="tex-span">[2, 3], [6, 4, 5, 7], [1]</span> with the values 3, 13 and 1 respectively.</p><p>In the fourth example one of the optimal partitions is <span class="tex-span">[1], [3, 4, 5, 5, 3, 4], [1]</span> with the values 1, 21 and 1 respectively.</p>
