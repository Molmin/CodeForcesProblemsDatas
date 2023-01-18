## Description

<div><p>Valera has got <span class="tex-span"><i>n</i></span> domino pieces in a row. Each piece consists of two halves — the upper one and the lower one. Each of the halves contains a number from <span class="tex-span">1</span> to <span class="tex-span">6</span>. Valera loves even integers very much, so he wants the sum of the numbers on the upper halves and the sum of the numbers on the lower halves to be even.</p><p>To do that, Valera can rotate the dominoes by <span class="tex-span">180</span> degrees. After the rotation the upper and the lower halves swap places. This action takes one second. Help Valera find out the minimum time he must spend rotating dominoes to make his wish come true.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>, denoting the number of dominoes Valera has. Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 6)</span>. Number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is initially written on the upper half of the <span class="tex-span"><i>i</i></span>-th domino, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is initially written on the lower half.</p></div><div class="output-specification"><p>Print a single number — the minimum required number of seconds. If Valera can't do the task in any time, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>, denoting the number of dominoes Valera has. Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 6)</span>. Number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is initially written on the upper half of the <span class="tex-span"><i>i</i></span>-th domino, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is initially written on the lower half.</p>

## Output

<p>Print a single number — the minimum required number of seconds. If Valera can't do the task in any time, print <span class="tex-span"> - 1</span>.</p>





```input1
2
4 2
6 4

```




```input2
1
2 3

```




```input3
3
1 4
2 3
4 4

```




```output1
0

```




```output2
-1

```




```output3
1

```



## Note

<p>In the first test case the sum of the numbers on the upper halves equals <span class="tex-span">10</span> and the sum of the numbers on the lower halves equals <span class="tex-span">6</span>. Both numbers are even, so Valera doesn't required to do anything.</p><p>In the second sample Valera has only one piece of domino. It is written <span class="tex-span">3</span> on the one of its halves, therefore one of the sums will always be odd.</p><p>In the third case Valera can rotate the first piece, and after that the sum on the upper halves will be equal to <span class="tex-span">10</span>, and the sum on the lower halves will be equal to <span class="tex-span">8</span>.</p>
