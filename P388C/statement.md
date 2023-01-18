## Description

<div><p>Fox Ciel is playing a card game with her friend Fox Jiro. There are <span class="tex-span"><i>n</i></span> piles of cards on the table. And there is a positive integer on each card.</p><p>The players take turns and Ciel takes the first turn. In Ciel's turn she takes a card from the top of any non-empty pile, and in Jiro's turn he takes a card from the bottom of any non-empty pile. Each player wants to maximize the total sum of the cards he took. The game ends when all piles become empty.</p><p>Suppose Ciel and Jiro play optimally, what is the score of the game?</p></div><div class="input-specification"><p>The first line contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains a description of the pile: the first integer in the line is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of cards in the <span class="tex-span"><i>i</i></span>-th pile; then follow <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> positive integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>s</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>k</i></sub> ≤ 1000</span>) — the sequence of the numbers on the cards listed from top of the current pile to bottom of the pile.</p></div><div class="output-specification"><p>Print two integers: the sum of Ciel's cards and the sum of Jiro's cards if they play optimally.</p></div>

## Input

<p>The first line contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains a description of the pile: the first integer in the line is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of cards in the <span class="tex-span"><i>i</i></span>-th pile; then follow <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> positive integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>s</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>k</i></sub> ≤ 1000</span>) — the sequence of the numbers on the cards listed from top of the current pile to bottom of the pile.</p>

## Output

<p>Print two integers: the sum of Ciel's cards and the sum of Jiro's cards if they play optimally.</p>





```input1
2
1 100
2 1 10

```




```input2
1
9 2 8 6 5 9 4 7 1 3

```




```input3
3
3 1 3 2
3 5 4 6
2 8 7

```




```input4
3
3 1000 1000 1000
6 1000 1000 1000 1000 1000 1000
5 1000 1000 1000 1000 1000

```




```output1
101 10

```




```output2
30 15

```




```output3
18 18

```




```output4
7000 7000

```



## Note

<p>In the first example, Ciel will take the cards with number 100 and 1, Jiro will take the card with number 10.</p><p>In the second example, Ciel will take cards with numbers 2, 8, 6, 5, 9 and Jiro will take cards with numbers 4, 7, 1, 3.</p>
