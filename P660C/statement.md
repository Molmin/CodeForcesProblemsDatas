## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> elements. Each element of <span class="tex-span"><i>a</i></span> is either <span class="tex-span">0</span> or <span class="tex-span">1</span>.</p><p>Let's denote the length of the longest subsegment of consecutive elements in <span class="tex-span"><i>a</i></span>, consisting of only numbers one, as <span class="tex-span"><i>f</i>(<i>a</i>)</span>. You can change no more than <span class="tex-span"><i>k</i></span> zeroes to ones to maximize <span class="tex-span"><i>f</i>(<i>a</i>)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of elements in <span class="tex-span"><i>a</i></span> and the parameter <span class="tex-span"><i>k</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — the elements of <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>On the first line print a non-negative integer <span class="tex-span"><i>z</i></span> — the maximal value of <span class="tex-span"><i>f</i>(<i>a</i>)</span> after no more than <span class="tex-span"><i>k</i></span> changes of zeroes to ones.</p><p>On the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> — the elements of the array <span class="tex-span"><i>a</i></span> after the changes.</p><p>If there are multiple answers, you can print any one of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of elements in <span class="tex-span"><i>a</i></span> and the parameter <span class="tex-span"><i>k</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — the elements of <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>On the first line print a non-negative integer <span class="tex-span"><i>z</i></span> — the maximal value of <span class="tex-span"><i>f</i>(<i>a</i>)</span> after no more than <span class="tex-span"><i>k</i></span> changes of zeroes to ones.</p><p>On the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> — the elements of the array <span class="tex-span"><i>a</i></span> after the changes.</p><p>If there are multiple answers, you can print any one of them.</p>





```input1
7 1
1 0 0 1 1 0 1

```




```input2
10 2
1 0 0 1 0 1 0 1 0 1

```




```output1
4
1 0 0 1 1 1 1

```




```output2
5
1 0 0 1 1 1 1 1 0 1

```


