## Description

<div><p>Little Gerald and his coach Mike play an interesting game. At the beginning of the game there is a pile consisting of <span class="tex-span"><i>n</i></span> candies and a pile consisting of <span class="tex-span"><i>m</i></span> stones. Gerald and Mike move in turns, Mike goes first. During his move Mike checks how many candies and stones Gerald has eaten. Let Gerald eat <span class="tex-span"><i>a</i></span> candies and <span class="tex-span"><i>b</i></span> stones. Then Mike awards Gerald <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>)</span> prize points. Gerald during his move either eats a candy from the pile of candies or a stone from the pile of stones. As Mike sees that Gerald has eaten everything apart one candy and one stone, he awards points for the last time and the game ends. Gerald is not allowed to eat all the candies, and he is not allowed to eat all the stones too. Tell Gerald how to play to get the largest possible number of points: it is required to find one of the possible optimal playing strategies for Gerald.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 20000</span>). The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 20000</span>). The value of <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>)</span> is calculated as a remainder of the division of the sum <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub> + <i>y</i><sub class="lower-index"><i>b</i></sub></span> by number <span class="tex-span"><i>p</i></span>.</p></div><div class="output-specification"><p>Print on the first line the only number: the maximal number of points Gerald can earn. Print on the second line a sting consisting of <span class="tex-span"><i>n</i> + <i>m</i> - 2</span> characters, each of which is either a "<span class="tex-font-style-tt">C</span>" or "<span class="tex-font-style-tt">S</span>", the <span class="tex-span"><i>i</i></span>-th character should be "<span class="tex-font-style-tt">C</span>" if Gerald's <span class="tex-span"><i>i</i></span>-th move should be eating a candy and "<span class="tex-font-style-tt">S</span>" if he should eat a stone.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 20000</span>). The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 20000</span>). The value of <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>)</span> is calculated as a remainder of the division of the sum <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub> + <i>y</i><sub class="lower-index"><i>b</i></sub></span> by number <span class="tex-span"><i>p</i></span>.</p>

## Output

<p>Print on the first line the only number: the maximal number of points Gerald can earn. Print on the second line a sting consisting of <span class="tex-span"><i>n</i> + <i>m</i> - 2</span> characters, each of which is either a "<span class="tex-font-style-tt">C</span>" or "<span class="tex-font-style-tt">S</span>", the <span class="tex-span"><i>i</i></span>-th character should be "<span class="tex-font-style-tt">C</span>" if Gerald's <span class="tex-span"><i>i</i></span>-th move should be eating a candy and "<span class="tex-font-style-tt">S</span>" if he should eat a stone.</p>





```input1
2 2 10
0 0
0 1

```




```input2
3 3 10
0 2 0
0 0 2

```




```input3
3 3 2
0 1 1
1 1 0

```




```output1
2
SC

```




```output2
10
CSSC

```




```output3
4
SCSC

```



## Note

<p>In the first test if Gerald's first move is eating a stone, he will receive a point for it and if he eats a candy, he will get zero pints. In any way Gerald will get <span class="tex-span">0</span> points before his first move, and <span class="tex-span">1</span> after his second one. This, the maximum number of points Gerald can get equals to <span class="tex-span">2</span>, and for that he should first eat a stone, then a candy.</p>
