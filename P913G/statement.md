## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>For every <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> you need to find a positive integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> such that the decimal notation of <span class="tex-span">2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup></span> contains the decimal notation of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> as a substring among its last <span class="tex-span"><i>min</i>(100, <i>length</i>(2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup>))</span> digits. Here <span class="tex-span"><i>length</i>(<i>m</i>)</span> is the length of the decimal notation of <span class="tex-span"><i>m</i></span>.</p><p>Note that you don't have to minimize <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. The decimal notations in this problem do not contain leading zeros.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 000</span>)&nbsp;— the number of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a positive integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">11</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain a positive integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> such that the last <span class="tex-span"><i>min</i>(100, <i>length</i>(2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup>))</span> digits of <span class="tex-span">2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup></span> contain the decimal notation of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> as a substring. Integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> must satisfy <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">50</sup></span>.</p><p>It can be shown that the answer always exists under the given constraints. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 000</span>)&nbsp;— the number of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a positive integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">11</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain a positive integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> such that the last <span class="tex-span"><i>min</i>(100, <i>length</i>(2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup>))</span> digits of <span class="tex-span">2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup></span> contain the decimal notation of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> as a substring. Integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> must satisfy <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">50</sup></span>.</p><p>It can be shown that the answer always exists under the given constraints. If there are multiple answers, print any of them.</p>





```input1
2
8
2

```




```input2
2
3
4857

```




```output1
3
1

```




```output2
5
20

```


