## Description

<div><p>Bike loves looking for the second maximum element in the sequence. The second maximum element in the sequence of distinct numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>k</i> &gt; 1)</span> is such maximum element <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, that the following inequality holds: <img align="middle" class="tex-formula" src="file://TQ9jP7a1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The lucky number of the sequence of distinct positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>k</i> &gt; 1)</span> is the number that is equal to the bitwise excluding OR of the maximum element of the sequence and the second maximum element of the sequence.</p><p>You've got a sequence of distinct positive integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>n</i> &gt; 1)</span>. Let's denote sequence <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub>, <i>s</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>s</i><sub class="lower-index"><i>r</i></sub></span> as <span class="tex-span"><i>s</i>[<i>l</i>..<i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i>)</span>. Your task is to find the maximum number among all lucky numbers of sequences <span class="tex-span"><i>s</i>[<i>l</i>..<i>r</i>]</span>.</p><p>Note that as all numbers in sequence <span class="tex-span"><i>s</i></span> are distinct, all the given definitions make sence.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the maximum lucky number among all lucky numbers of sequences <span class="tex-span"><i>s</i>[<i>l</i>..<i>r</i>]</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print a single integer — the maximum lucky number among all lucky numbers of sequences <span class="tex-span"><i>s</i>[<i>l</i>..<i>r</i>]</span>.</p>





```input1
5
5 2 1 4 3

```




```input2
5
9 8 3 5 7

```




```output1
7

```




```output2
15

```



## Note

<p>For the first sample you can choose <span class="tex-span"><i>s</i>[4..5] = {4, 3}</span> and its lucky number is <span class="tex-span">(4&nbsp;<i>xor</i>&nbsp;3) = 7</span>. You can also choose <span class="tex-span"><i>s</i>[1..2]</span>.</p><p>For the second sample you must choose <span class="tex-span"><i>s</i>[2..5] = {8, 3, 5, 7}</span>.</p>
