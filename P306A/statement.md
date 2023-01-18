## Description

<div><p>Polycarpus has got <span class="tex-span"><i>n</i></span> candies and <span class="tex-span"><i>m</i></span> friends (<span class="tex-span"><i>n</i> ≥ <i>m</i></span>). He wants to make a New Year present with candies to each friend. Polycarpus is planning to present all candies and he wants to do this in the fairest (that is, most equal) manner. He wants to choose such <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of candies in the <span class="tex-span"><i>i</i></span>-th friend's present, that the maximum <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> differs from the least <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> as little as possible.</p><p>For example, if <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>m</i></span>, then he is going to present the same number of candies to all his friends, that is, the maximum <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> won't differ from the minimum one.</p></div><div class="input-specification"><p>The single line of the input contains a pair of space-separated positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100;<i>n</i> ≥ <i>m</i></span>) — the number of candies and the number of Polycarpus's friends.</p></div><div class="output-specification"><p>Print the required sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of candies in the <span class="tex-span"><i>i</i></span>-th friend's present. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must be positive integers, total up to <span class="tex-span"><i>n</i></span>, the maximum one should differ from the minimum one by the smallest possible value.</p></div>

## Input

<p>The single line of the input contains a pair of space-separated positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100;<i>n</i> ≥ <i>m</i></span>) — the number of candies and the number of Polycarpus's friends.</p>

## Output

<p>Print the required sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of candies in the <span class="tex-span"><i>i</i></span>-th friend's present. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must be positive integers, total up to <span class="tex-span"><i>n</i></span>, the maximum one should differ from the minimum one by the smallest possible value.</p>





```input1
12 3

```




```input2
15 4

```




```input3
18 7

```




```output1
4 4 4
```




```output2
3 4 4 4
```




```output3
2 2 2 3 3 3 3
```



## Note

<p>Print <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> in any order, separate the numbers by spaces.</p>
