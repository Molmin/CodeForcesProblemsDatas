## Description

<div><p>Blake is a CEO of a large company called "Blake Technologies". He loves his company very much and he thinks that his company should be the best. That is why every candidate needs to pass through the interview that consists of the following problem.</p><p>We define function <span class="tex-span"><i>f</i>(<i>x</i>, <i>l</i>, <i>r</i>)</span> as a bitwise OR of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>l</i></sub>, <i>x</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>x</i><sub class="lower-index"><i>r</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the array <span class="tex-span"><i>x</i></span>. You are given two arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span>. You need to determine the maximum value of sum <span class="tex-span"><i>f</i>(<i>a</i>, <i>l</i>, <i>r</i>) + <i>f</i>(<i>b</i>, <i>l</i>, <i>r</i>)</span> among all possible <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>.</p><center> <img class="tex-graphics" src="file://Nmx5rHcu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the length of the arrays.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum value of sum <span class="tex-span"><i>f</i>(<i>a</i>, <i>l</i>, <i>r</i>) + <i>f</i>(<i>b</i>, <i>l</i>, <i>r</i>)</span> among all possible <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the length of the arrays.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single integer&nbsp;— the maximum value of sum <span class="tex-span"><i>f</i>(<i>a</i>, <i>l</i>, <i>r</i>) + <i>f</i>(<i>b</i>, <i>l</i>, <i>r</i>)</span> among all possible <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>.</p>





```input1
5
1 2 4 3 2
2 3 3 12 1

```




```input2
10
13 2 7 11 8 4 9 8 5 1
5 7 18 9 2 3 0 11 8 6

```




```output1
22
```




```output2
46
```



## Note

<p>Bitwise OR of two non-negative integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is the number <span class="tex-span"><i>c</i> = <i>a</i> <i>OR</i> <i>b</i></span>, such that each of its digits in binary notation is <span class="tex-span">1</span> if and only if at least one of <span class="tex-span"><i>a</i></span> or <span class="tex-span"><i>b</i></span> have <span class="tex-span">1</span> in the corresponding position in binary notation.</p><p>In the first sample, one of the optimal answers is <span class="tex-span"><i>l</i> = 2</span> and <span class="tex-span"><i>r</i> = 4</span>, because <span class="tex-span"><i>f</i>(<i>a</i>, 2, 4) + <i>f</i>(<i>b</i>, 2, 4) = (2 <i>OR</i> 4 <i>OR</i> 3) + (3 <i>OR</i> 3 <i>OR</i> 12) = 7 + 15 = 22</span>. Other ways to get maximum value is to choose <span class="tex-span"><i>l</i> = 1</span> and <span class="tex-span"><i>r</i> = 4</span>, <span class="tex-span"><i>l</i> = 1</span> and <span class="tex-span"><i>r</i> = 5</span>, <span class="tex-span"><i>l</i> = 2</span> and <span class="tex-span"><i>r</i> = 4</span>, <span class="tex-span"><i>l</i> = 2</span> and <span class="tex-span"><i>r</i> = 5</span>, <span class="tex-span"><i>l</i> = 3</span> and <span class="tex-span"><i>r</i> = 4</span>, or <span class="tex-span"><i>l</i> = 3</span> and <span class="tex-span"><i>r</i> = 5</span>.</p><p>In the second sample, the maximum value is obtained for <span class="tex-span"><i>l</i> = 1</span> and <span class="tex-span"><i>r</i> = 9</span>.</p>
