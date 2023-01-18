## Description

<div><p>Anton goes to school, his favorite lessons are arraystudying. He usually solves all the tasks pretty fast, but this time the teacher gave him a complicated one: given two arrays <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> of length <span class="tex-span"><i>n</i></span>, find array <span class="tex-span"><i>a</i></span>, such that:</p><p><img align="middle" class="tex-formula" src="file://u0LkMTQR.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>where <span class="tex-span"><i>a</i>&nbsp;<i>and</i>&nbsp;<i>b</i></span> means bitwise AND, while <span class="tex-span"><i>a</i>&nbsp;<i>or</i>&nbsp;<i>b</i></span> means bitwise OR.</p><p>Usually Anton is good in arraystudying, but this problem is too hard, so Anton asks you to help.</p></div><div class="input-specification"><p>The first line of the input contains a single integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the size of arrays <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array <span class="tex-span"><i>b</i></span>.</p><p>Third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array <span class="tex-span"><i>c</i></span>.</p></div><div class="output-specification"><p>If there is no solution, print <span class="tex-span"> - 1</span>.</p><p>Otherwise, the only line of the output should contain <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— elements of the array <span class="tex-span"><i>a</i></span>. If there are multiple possible solutions, you may print any of them.</p></div>

## Input

<p>The first line of the input contains a single integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the size of arrays <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array <span class="tex-span"><i>b</i></span>.</p><p>Third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array <span class="tex-span"><i>c</i></span>.</p>

## Output

<p>If there is no solution, print <span class="tex-span"> - 1</span>.</p><p>Otherwise, the only line of the output should contain <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— elements of the array <span class="tex-span"><i>a</i></span>. If there are multiple possible solutions, you may print any of them.</p>





```input1
4
6 8 4 4
16 22 10 10

```




```input2
5
8 25 14 7 16
19 6 9 4 25

```




```output1
3 5 1 1 

```




```output2
-1

```


