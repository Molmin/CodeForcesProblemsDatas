## Description

<div><p>Let's denote a function </p><p><img align="middle" class="tex-formula" src="file://rcSwnHhd.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. You have to calculate the sum of <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> over all pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of the array. </p></div><div class="output-specification"><p>Print one integer — the sum of <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> over all pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of the array. </p>

## Output

<p>Print one integer — the sum of <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> over all pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>.</p>





```input1
5
1 2 3 1 3

```




```input2
4
6 6 5 5

```




```input3
4
6 6 4 4

```




```output1
4

```




```output2
0

```




```output3
-8

```



## Note

<p>In the first example:</p><ol> <li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>) = 0</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">3</sub>) = 2</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">4</sub>) = 0</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">5</sub>) = 2</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>) = 0</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">4</sub>) = 0</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">5</sub>) = 0</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>) =  - 2</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">5</sub>) = 0</span>; </li><li> <span class="tex-span"><i>d</i>(<i>a</i><sub class="lower-index">4</sub>, <i>a</i><sub class="lower-index">5</sub>) = 2</span>. </li></ol>
