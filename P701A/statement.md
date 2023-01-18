## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cards (<span class="tex-span"><i>n</i></span> is <span class="tex-font-style-bf">even</span>) in the deck. Each card has a positive integer written on it. <span class="tex-span"><i>n</i> / 2</span> people will play new card game. At the beginning of the game each player gets two cards, each card is given to exactly one player. </p><p>Find the way to distribute cards such that the sum of values written of the cards will be equal for each player. It is guaranteed that it is always possible.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of cards in the deck. It is guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>The second line contains the sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number written on the <span class="tex-span"><i>i</i></span>-th card.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> / 2</span> pairs of integers, the <span class="tex-span"><i>i</i></span>-th pair denote the cards that should be given to the <span class="tex-span"><i>i</i></span>-th player. Each card should be given to exactly one player. Cards are numbered in the order they appear in the input.</p><p>It is guaranteed that solution exists. If there are several correct answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of cards in the deck. It is guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>The second line contains the sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number written on the <span class="tex-span"><i>i</i></span>-th card.</p>

## Output

<p>Print <span class="tex-span"><i>n</i> / 2</span> pairs of integers, the <span class="tex-span"><i>i</i></span>-th pair denote the cards that should be given to the <span class="tex-span"><i>i</i></span>-th player. Each card should be given to exactly one player. Cards are numbered in the order they appear in the input.</p><p>It is guaranteed that solution exists. If there are several correct answers, you are allowed to print any of them.</p>





```input1
6
1 5 7 4 4 3

```




```input2
4
10 10 10 10

```




```output1
1 3
6 2
4 5

```




```output2
1 2
3 4

```



## Note

<p>In the first sample, cards are distributed in such a way that each player has the sum of numbers written on his cards equal to <span class="tex-span">8</span>. </p><p>In the second sample, all values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are equal. Thus, any distribution is acceptable.</p>
