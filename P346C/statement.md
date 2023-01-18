## Description

<div><p>You are given a sequence of positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> and two non-negative integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Your task is to transform <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span>. To do that, you can perform the following moves:</p><ul> <li> subtract 1 from the current <span class="tex-span"><i>a</i></span>; </li><li> subtract <span class="tex-span"><i>a</i></span> mod <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> from the current <span class="tex-span"><i>a</i></span>. </li></ul><p>Operation <span class="tex-span"><i>a</i></span> mod <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> means taking the remainder after division of number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Now you want to know the minimum number of moves needed to transform <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤  <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤  <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0  ≤ <i>b</i> ≤  <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i> - <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print a single integer — the required minimum number of moves needed to transform number <span class="tex-span"><i>a</i></span> into number <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤  <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤  <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0  ≤ <i>b</i> ≤  <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i> - <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print a single integer — the required minimum number of moves needed to transform number <span class="tex-span"><i>a</i></span> into number <span class="tex-span"><i>b</i></span>.</p>





```input1
3
3 4 5
30 17

```




```input2
3
5 6 7
1000 200

```




```output1
6

```




```output2
206

```


