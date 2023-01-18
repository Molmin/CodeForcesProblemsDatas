## Description

<div><p>There is an infinite sequence consisting of all positive integers in the increasing order: <span class="tex-span"><i>p</i> = {1, 2, 3, ...}</span>. We performed <span class="tex-span"><i>n</i></span> <span class="tex-font-style-it">swap</span> operations with this sequence. A <span class="tex-span"><i>swap</i>(<i>a</i>, <i>b</i>)</span> is an operation of swapping the elements of the sequence on positions <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Your task is to find the number of inversions in the resulting sequence, i.e. the number of such index pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &gt; <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of <span class="tex-font-style-it">swap</span> operations applied to the sequence.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the arguments of the <span class="tex-font-style-it">swap</span> operation.</p></div><div class="output-specification"><p>Print a single integer — the number of inversions in the resulting sequence.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of <span class="tex-font-style-it">swap</span> operations applied to the sequence.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the arguments of the <span class="tex-font-style-it">swap</span> operation.</p>

## Output

<p>Print a single integer — the number of inversions in the resulting sequence.</p>





```input1
2
4 2
1 4

```




```input2
3
1 6
3 4
2 5

```




```output1
4

```




```output2
15

```



## Note

<p>In the first sample the sequence is being modified as follows: <img align="middle" class="tex-formula" src="file://47BeNZiK.png" style="max-width: 100.0%;max-height: 100.0%;">. It has 4 inversions formed by index pairs <span class="tex-span">(1, 4)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(2, 4)</span> and <span class="tex-span">(3, 4)</span>.</p>
