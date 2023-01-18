## Description

<div><p>Vasily has a deck of cards consisting of <span class="tex-span"><i>n</i></span> cards. There is an integer on each of the cards, this integer is between <span class="tex-span">1</span> and <span class="tex-span">100 000</span>, inclusive. It is possible that some cards have the same integers on them.</p><p>Vasily decided to sort the cards. To do this, he repeatedly takes the top card from the deck, and if the number on it equals the minimum number written on the cards in the deck, then he places the card away. Otherwise, he puts it under the deck and takes the next card from the top, and so on. The process ends as soon as there are no cards in the deck. You can assume that Vasily always knows the minimum number written on some card in the remaining deck, but doesn't know where this card (or these cards) is.</p><p>You are to determine the total number of times Vasily takes the top card from the deck.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of cards in the deck.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number written on the <span class="tex-span"><i>i</i></span>-th from top card in the deck.</p></div><div class="output-specification"><p>Print the total number of times Vasily takes the top card from the deck.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of cards in the deck.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number written on the <span class="tex-span"><i>i</i></span>-th from top card in the deck.</p>

## Output

<p>Print the total number of times Vasily takes the top card from the deck.</p>





```input1
4
6 3 1 2

```




```input2
1
1000

```




```input3
7
3 3 3 3 3 3 3

```




```output1
7

```




```output2
1

```




```output3
7

```



## Note

<p>In the first example Vasily at first looks at the card with number <span class="tex-span">6</span> on it, puts it under the deck, then on the card with number <span class="tex-span">3</span>, puts it under the deck, and then on the card with number <span class="tex-span">1</span>. He places away the card with <span class="tex-span">1</span>, because the number written on it is the minimum among the remaining cards. After that the cards from top to bottom are <span class="tex-span">[2, 6, 3]</span>. Then Vasily looks at the top card with number <span class="tex-span">2</span> and puts it away. After that the cards from top to bottom are <span class="tex-span">[6, 3]</span>. Then Vasily looks at card <span class="tex-span">6</span>, puts it under the deck, then at card <span class="tex-span">3</span> and puts it away. Then there is only one card with number <span class="tex-span">6</span> on it, and Vasily looks at it and puts it away. Thus, in total Vasily looks at <span class="tex-span">7</span> cards.</p>
