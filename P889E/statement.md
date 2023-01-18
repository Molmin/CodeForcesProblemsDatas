## Description

<div><p>You are given a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Let <img align="middle" class="tex-formula" src="file://e8TFwI7i.png" style="max-width: 100.0%;max-height: 100.0%;">, and <img align="middle" class="tex-formula" src="file://tZY39MjC.png" style="max-width: 100.0%;max-height: 100.0%;"> for <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>. Here, <img align="middle" class="tex-formula" src="file://VjUSHDdV.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the modulus operation. Find the maximum value of <span class="tex-span"><i>f</i>(<i>x</i>, 1)</span> over all nonnegative integers <span class="tex-span"><i>x</i></span>. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>)&nbsp;— the length of the sequence.</p><p>The second lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">13</sup></span>)&nbsp;— the elements of the sequence.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the maximum value of <span class="tex-span"><i>f</i>(<i>x</i>, 1)</span> over all nonnegative integers <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>)&nbsp;— the length of the sequence.</p><p>The second lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">13</sup></span>)&nbsp;— the elements of the sequence.</p>

## Output

<p>Output a single integer&nbsp;— the maximum value of <span class="tex-span"><i>f</i>(<i>x</i>, 1)</span> over all nonnegative integers <span class="tex-span"><i>x</i></span>.</p>





```input1
2
10 5

```




```input2
5
5 4 3 2 1

```




```input3
4
5 10 5 10

```




```output1
13

```




```output2
6

```




```output3
16

```



## Note

<p>In the first example you can choose, for example, <span class="tex-span"><i>x</i> = 19</span>.</p><p>In the second example you can choose, for example, <span class="tex-span"><i>x</i> = 3</span> or <span class="tex-span"><i>x</i> = 2</span>.</p>
