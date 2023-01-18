## Description

<div><p>Yash has recently learnt about the Fibonacci sequence and is very excited about it. He calls a sequence Fibonacci-ish if </p><ol> <li> the sequence consists of at least two elements </li><li> <span class="tex-span"><i>f</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span> are arbitrary </li><li> <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i> + 2</sub> = <i>f</i><sub class="lower-index"><i>n</i> + 1</sub> + <i>f</i><sub class="lower-index"><i>n</i></sub></span> for all <span class="tex-span"><i>n</i> ≥ 0</span>. </li></ol><p>You are given some sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Your task is rearrange elements of this sequence in such a way that its longest possible prefix is Fibonacci-ish sequence.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the length of the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the length of the longest possible Fibonacci-ish prefix of the given sequence after rearrangement.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the length of the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the length of the longest possible Fibonacci-ish prefix of the given sequence after rearrangement.</p>





```input1
3
1 2 -1

```




```input2
5
28 35 7 14 21

```




```output1
3

```




```output2
4

```



## Note

<p>In the first sample, if we rearrange elements of the sequence as <span class="tex-span"> - 1</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span>, the whole sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> would be Fibonacci-ish.</p><p>In the second sample, the optimal way to rearrange elements is <img align="middle" class="tex-formula" src="file://GsxUDlsR.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://6FJSNZkY.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://fl9dh7XC.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://ICGQl9vw.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">28</span>.</p>
