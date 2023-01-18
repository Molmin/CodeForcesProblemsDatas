## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> distinct integers. Construct an array <span class="tex-span"><i>b</i></span> by permuting <span class="tex-span"><i>a</i></span> such that for every non-empty subset of indices <span class="tex-span"><i>S</i> = {<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub>}</span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 &lt; <i>k</i> &lt; <i>n</i></span>) the sums of elements on that positions in <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are different, i.&nbsp;e. </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://99skj7tz.png" style="max-width: 100.0%;max-height: 100.0%;"></center></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 22</span>)&nbsp;— the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>If there is no such array <span class="tex-span"><i>b</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise in the only line print <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. Note that <span class="tex-span"><i>b</i></span> must be a permutation of <span class="tex-span"><i>a</i></span>.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 22</span>)&nbsp;— the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array.</p>

## Output

<p>If there is no such array <span class="tex-span"><i>b</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise in the only line print <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. Note that <span class="tex-span"><i>b</i></span> must be a permutation of <span class="tex-span"><i>a</i></span>.</p><p>If there are multiple answers, print any of them.</p>





```input1
2
1 2

```




```input2
4
1000 100 10 1

```




```output1
2 1 

```




```output2
100 1 1000 10

```



## Note

<p>An array <span class="tex-span"><i>x</i></span> is a permutation of <span class="tex-span"><i>y</i></span>, if we can shuffle elements of <span class="tex-span"><i>y</i></span> such that it will coincide with <span class="tex-span"><i>x</i></span>.</p><p>Note that the empty subset and the subset containing all indices are not counted.</p>
