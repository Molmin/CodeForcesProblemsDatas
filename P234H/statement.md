## Description

<div><p>There are two decks of cards lying on the table in front of you, some cards in these decks lay face up, some of them lay face down. You want to merge them into one deck in which each card is face down. You're going to do it in two stages.</p><p>The first stage is to merge the two decks in such a way that the relative order of the cards from the same deck doesn't change. That is, for any two different cards <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> in one deck, if card <span class="tex-span"><i>i</i></span> lies above card <span class="tex-span"><i>j</i></span>, then after the merge card <span class="tex-span"><i>i</i></span> must also be above card <span class="tex-span"><i>j</i></span>.</p><p>The second stage is performed on the deck that resulted from the first stage. At this stage, the executed operation is the turning operation. In one turn you can take a few of the top cards, turn all of them, and put them back. Thus, each of the taken cards gets turned and the order of these cards is reversed. That is, the card that was on the bottom before the turn, will be on top after it.</p><p>Your task is to make sure that all the cards are lying face down. Find such an order of merging cards in the first stage and the sequence of turning operations in the second stage, that make all the cards lie face down, and the number of turns is minimum.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> — the number of cards in the first deck <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The second input line contains <span class="tex-span"><i>n</i></span> integers, separated by single spaces <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>. Value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 0, if the <span class="tex-span"><i>i</i></span>-th card is lying face down, and 1, if the card is lying face up. The cards are given in the order from the topmost one to the bottommost one.</p><p>The third input line contains integer <span class="tex-span"><i>m</i></span> — the number of cards in the second deck <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The fourth input line contains <span class="tex-span"><i>m</i></span> integers, separated by single spaces <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>. Value <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals 0, if the <span class="tex-span"><i>i</i></span>-th card is lying face down, and 1, if the card is lying face up. The cards are given in the order from the topmost to the bottommost.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>n</i> + <i>m</i></span> space-separated integers — the numbers of the cards in the order, in which they will lie after the first stage. List the cards from top to bottom. The cards from the first deck should match their indexes from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order from top to bottom. The cards from the second deck should match their indexes, increased by <span class="tex-span"><i>n</i></span>, that is, numbers from <span class="tex-span"><i>n</i> + 1</span> to <span class="tex-span"><i>n</i> + <i>m</i></span> in the order from top to bottom.</p><p>In the second line print a single integer <span class="tex-span"><i>x</i></span> — the minimum number of turn operations you need to make all cards in the deck lie face down. In the third line print <span class="tex-span"><i>x</i></span> integers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>x</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> + <i>m</i>)</span>, each of them represents the number of cards to take from the top of the deck to perform a turn operation. Print the operations in the order, in which they should be performed. </p><p>If there are multiple optimal solutions, print any of them. It is guaranteed that the minimum number of operations doesn't exceed <span class="tex-span">6·10<sup class="upper-index">5</sup></span>. </p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> — the number of cards in the first deck <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The second input line contains <span class="tex-span"><i>n</i></span> integers, separated by single spaces <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>. Value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 0, if the <span class="tex-span"><i>i</i></span>-th card is lying face down, and 1, if the card is lying face up. The cards are given in the order from the topmost one to the bottommost one.</p><p>The third input line contains integer <span class="tex-span"><i>m</i></span> — the number of cards in the second deck <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The fourth input line contains <span class="tex-span"><i>m</i></span> integers, separated by single spaces <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>. Value <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals 0, if the <span class="tex-span"><i>i</i></span>-th card is lying face down, and 1, if the card is lying face up. The cards are given in the order from the topmost to the bottommost.</p>

## Output

<p>In the first line print <span class="tex-span"><i>n</i> + <i>m</i></span> space-separated integers — the numbers of the cards in the order, in which they will lie after the first stage. List the cards from top to bottom. The cards from the first deck should match their indexes from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order from top to bottom. The cards from the second deck should match their indexes, increased by <span class="tex-span"><i>n</i></span>, that is, numbers from <span class="tex-span"><i>n</i> + 1</span> to <span class="tex-span"><i>n</i> + <i>m</i></span> in the order from top to bottom.</p><p>In the second line print a single integer <span class="tex-span"><i>x</i></span> — the minimum number of turn operations you need to make all cards in the deck lie face down. In the third line print <span class="tex-span"><i>x</i></span> integers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>x</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> + <i>m</i>)</span>, each of them represents the number of cards to take from the top of the deck to perform a turn operation. Print the operations in the order, in which they should be performed. </p><p>If there are multiple optimal solutions, print any of them. It is guaranteed that the minimum number of operations doesn't exceed <span class="tex-span">6·10<sup class="upper-index">5</sup></span>. </p>





```input1
3
1 0 1
4
1 1 1 1

```




```input2
5
1 1 1 1 1
5
0 1 0 1 0

```




```output1
1 4 5 6 7 2 3
3
5 6 7

```




```output2
6 1 2 3 4 5 7 8 9 10
4
1 7 8 9

```


