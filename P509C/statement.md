## Description

<div><p>Vasya had a <span class="tex-font-style-bf">strictly increasing</span> sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. Vasya used it to build a new sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the sum of digits of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s decimal representation. Then sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> got lost and all that remained is sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Vasya wonders what the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> could be like. Of all the possible options he likes the one sequence with the minimum possible last number <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. Help Vasya restore the initial sequence.</p><p>It is guaranteed that such a sequence always exists.</p></div><div class="input-specification"><p>The first line contains a single integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> &nbsp;— the required sums of digits. All <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> belong to the range <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 300</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integer numbers, one per line&nbsp;— the correct option for numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, in order of following in sequence. The sequence should be strictly increasing. The sum of digits of the <span class="tex-span"><i>i</i></span>-th number should be equal to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>If there are multiple sequences with least possible number <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, print any of them. Print the numbers without leading zeroes.</p></div>

## Input

<p>The first line contains a single integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> &nbsp;— the required sums of digits. All <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> belong to the range <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 300</span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integer numbers, one per line&nbsp;— the correct option for numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, in order of following in sequence. The sequence should be strictly increasing. The sum of digits of the <span class="tex-span"><i>i</i></span>-th number should be equal to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>If there are multiple sequences with least possible number <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, print any of them. Print the numbers without leading zeroes.</p>





```input1
3
1
2
3

```




```input2
3
3
2
1

```




```output1
1
2
3

```




```output2
3
11
100

```


