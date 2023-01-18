## Description

<div><p>You are given a sequence <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. You may partition this sequence into two sequences <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> in such a way that every element belongs exactly to one of these sequences. </p><p>Let <span class="tex-span"><i>B</i></span> be the sum of elements belonging to <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>C</i></span> be the sum of elements belonging to <span class="tex-span"><i>c</i></span> (if some of these sequences is empty, then its sum is <span class="tex-span">0</span>). What is the maximum possible value of <span class="tex-span"><i>B</i> - <i>C</i></span>?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of sequence <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print the maximum possible value of <span class="tex-span"><i>B</i> - <i>C</i></span>, where <span class="tex-span"><i>B</i></span> is the sum of elements of sequence <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>C</i></span> is the sum of elements of sequence <span class="tex-span"><i>c</i></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of sequence <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print the maximum possible value of <span class="tex-span"><i>B</i> - <i>C</i></span>, where <span class="tex-span"><i>B</i></span> is the sum of elements of sequence <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>C</i></span> is the sum of elements of sequence <span class="tex-span"><i>c</i></span>.</p>





```input1
3
1 -2 0

```




```input2
6
16 23 16 15 42 8

```




```output1
3

```




```output2
120

```



## Note

<p>In the first example we may choose <span class="tex-span"><i>b</i> = {1, 0}</span>, <span class="tex-span"><i>c</i> = { - 2}</span>. Then <span class="tex-span"><i>B</i> = 1</span>, <span class="tex-span"><i>C</i> =  - 2</span>, <span class="tex-span"><i>B</i> - <i>C</i> = 3</span>.</p><p>In the second example we choose <span class="tex-span"><i>b</i> = {16, 23, 16, 15, 42, 8}</span>, <span class="tex-span"><i>c</i> = {}</span> (an empty sequence). Then <span class="tex-span"><i>B</i> = 120</span>, <span class="tex-span"><i>C</i> = 0</span>, <span class="tex-span"><i>B</i> - <i>C</i> = 120</span>.</p>
