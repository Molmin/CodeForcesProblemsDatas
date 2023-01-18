## Description

<div><p>Fox Ciel is playing a game with numbers now. </p><p>Ciel has <span class="tex-span"><i>n</i></span> positive integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span>. She can do the following operation as many times as needed: select two different indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> &gt; <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> hold, and then apply assignment <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> = <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> - <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>. The goal is to make the sum of all numbers as small as possible.</p><p>Please help Ciel to find this minimal sum.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). Then the second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Output a single integer — the required minimal sum.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). Then the second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Output a single integer — the required minimal sum.</p>





```input1
2
1 2

```




```input2
3
2 4 6

```




```input3
2
12 18

```




```input4
5
45 12 27 30 18

```




```output1
2

```




```output2
6

```




```output3
12

```




```output4
15

```



## Note

<p>In the first example the optimal way is to do the assignment: <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> = <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> - <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>.</p><p>In the second example the optimal sequence of operations is: <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span> = <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span> - <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> = <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> - <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>.</p>
