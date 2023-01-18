## Description

<div><p>As you know, the game of "Nim" is played with <span class="tex-span"><i>n</i></span> piles of stones, where the <span class="tex-span"><i>i</i></span>-th pile initially contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stones. Two players alternate the turns. During a turn a player picks any non-empty pile and removes any positive number of stones from it. The one who is not able to make a move loses the game.</p><p>Petya and Vasya are tired of playing Nim, so they invented their own version of the game and named it the "Gambling Nim". They have <span class="tex-span"><i>n</i></span> two-sided cards, one side of the <span class="tex-span"><i>i</i></span>-th card has number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> written on it, while the other side has number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. At the beginning of the game the players put all the cards on the table, each card only one of its sides up, and this side is chosen independently and uniformly. Thus they obtain a sequence <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Then they take <span class="tex-span"><i>n</i></span> piles of stones, with <span class="tex-span"><i>i</i></span>-th pile containing exactly <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> stones and play Nim. Petya takes the first turn.</p><p>Given that both players play optimally, find the probability of Petya's victory. Output the answer as an irreducible fraction.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the number of cards in the deck.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains the description of one card, consisting of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Output the answer as an irreducible fraction <span class="tex-span"><i>p</i> / <i>q</i></span>. If the probability of Petya's victory is <span class="tex-span">0</span>, print <span class="tex-font-style-tt">0/1</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the number of cards in the deck.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains the description of one card, consisting of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Output the answer as an irreducible fraction <span class="tex-span"><i>p</i> / <i>q</i></span>. If the probability of Petya's victory is <span class="tex-span">0</span>, print <span class="tex-font-style-tt">0/1</span>.</p>





```input1
2
1 1
1 1

```




```input2
2
1 2
1 2

```




```input3
3
0 4
1 5
2 3

```




```output1
0/1

```




```output2
1/2

```




```output3
1/1

```


