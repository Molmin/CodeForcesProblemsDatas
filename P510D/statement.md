## Description

<div><p>Fox Ciel is playing a game. In this game there is an infinite long tape with cells indexed by integers (positive, negative and zero). At the beginning she is standing at the cell 0.</p><p>There are also <span class="tex-span"><i>n</i></span> cards, each card has 2 attributes: length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. If she pays <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> dollars then she can apply <span class="tex-span"><i>i</i></span>-th card. After applying <span class="tex-span"><i>i</i></span>-th card she becomes able to make jumps of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, i. e. from cell <span class="tex-span"><i>x</i></span> to cell <span class="tex-span">(<i>x</i> - <i>l</i><sub class="lower-index"><i>i</i></sub>)</span> or cell <span class="tex-span">(<i>x</i> + <i>l</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>She wants to be able to jump to any cell on the tape (possibly, visiting some intermediate cells). For achieving this goal, she wants to buy some cards, paying as little money as possible. </p><p>If this is possible, calculate the minimal cost.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>), number of cards.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the jump lengths of cards.</p><p>The third line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), the costs of cards.</p></div><div class="output-specification"><p>If it is impossible to buy some cards and become able to jump to any cell, output -1. Otherwise output the minimal cost of buying such set of cards.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>), number of cards.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the jump lengths of cards.</p><p>The third line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), the costs of cards.</p>

## Output

<p>If it is impossible to buy some cards and become able to jump to any cell, output -1. Otherwise output the minimal cost of buying such set of cards.</p>





```input1
3
100 99 9900
1 1 1

```




```input2
5
10 20 30 40 50
1 1 1 1 1

```




```input3
7
15015 10010 6006 4290 2730 2310 1
1 1 1 1 1 1 10

```




```input4
8
4264 4921 6321 6984 2316 8432 6120 1026
4264 4921 6321 6984 2316 8432 6120 1026

```




```output1
2

```




```output2
-1

```




```output3
6

```




```output4
7237

```



## Note

<p>In first sample test, buying one card is not enough: for example, if you buy a card with length 100, you can't jump to any cell whose index is not a multiple of 100. The best way is to buy first and second card, that will make you be able to jump to any cell.</p><p>In the second sample test, even if you buy all cards, you can't jump to any cell whose index is not a multiple of 10, so you should output -1.</p>
