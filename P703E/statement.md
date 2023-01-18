## Description

<div><p>After playing with her beautiful array, Mishka decided to learn some math. After learning how to multiply, divide and what is divisibility, she is now interested in solving the following problem.</p><p>You are given integer <span class="tex-span"><i>k</i></span> and array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of <span class="tex-span"><i>n</i></span> integers. You are to find <span class="tex-font-style-bf">non-empty</span> subsequence of array elements such that the product of its elements is divisible by <span class="tex-span"><i>k</i></span> and it contains minimum possible number of elements.</p><p>Formally, you are to find a sequence of indices <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>m</i></sub> ≤ <i>n</i></span> such that <img align="middle" class="tex-formula" src="file://IISX9C5e.png" style="max-width: 100.0%;max-height: 100.0%;"> is divisible by <span class="tex-span"><i>k</i></span> while <span class="tex-span"><i>m</i></span> is minimum possible among all such variants.</p><p>If there are more than one such subsequences, you should choose one among them, such that sum of its elements is <span class="tex-font-style-bf">minimum possible</span>.</p><p>Mishka quickly solved this problem. Will you do so?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>).</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>)&nbsp;— array elements.</p></div><div class="output-specification"><p>Print single positive integer <span class="tex-span"><i>m</i></span> in the first line&nbsp;— the number of elements in desired sequence.</p><p>In the second line print <span class="tex-span"><i>m</i></span> distinct integers&nbsp;— the sequence of indices of given array elements, which should be taken into the desired sequence. </p><p>If there are more than one such subsequence (e.g. subsequence of minimum possible number of elements and with minimum possible sum of elements), you can print any of them.</p><p>If there are no such subsequences, print <span class="tex-span"> - 1</span> in the only line.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>).</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>)&nbsp;— array elements.</p>

## Output

<p>Print single positive integer <span class="tex-span"><i>m</i></span> in the first line&nbsp;— the number of elements in desired sequence.</p><p>In the second line print <span class="tex-span"><i>m</i></span> distinct integers&nbsp;— the sequence of indices of given array elements, which should be taken into the desired sequence. </p><p>If there are more than one such subsequence (e.g. subsequence of minimum possible number of elements and with minimum possible sum of elements), you can print any of them.</p><p>If there are no such subsequences, print <span class="tex-span"> - 1</span> in the only line.</p>





```input1
5 60
2 4 6 5 2

```




```output1
3
4 3 1
```


