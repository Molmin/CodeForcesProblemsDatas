## Description

<div><p>Vova again tries to play some computer card game.</p><p>The rules of deck creation in this game are simple. Vova is given an existing deck of <span class="tex-span"><i>n</i></span> cards and a magic number <span class="tex-span"><i>k</i></span>. The order of the cards in the deck is fixed. Each card has a number written on it; number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is written on the <span class="tex-span"><i>i</i></span>-th card in the deck.</p><p>After receiving the deck and the magic number, Vova removes <span class="tex-span"><i>x</i></span> (possibly <span class="tex-span"><i>x</i> = 0</span>) cards from the top of the deck, <span class="tex-span"><i>y</i></span> (possibly <span class="tex-span"><i>y</i> = 0</span>) cards from the bottom of the deck, and the rest of the deck is his new deck (Vova has to leave at least one card in the deck after removing cards). So Vova's new deck actually contains cards <span class="tex-span"><i>x</i> + 1</span>, <span class="tex-span"><i>x</i> + 2</span>, ... <span class="tex-span"><i>n</i> - <i>y</i> - 1</span>, <span class="tex-span"><i>n</i> - <i>y</i></span> from the original deck.</p><p>Vova's new deck is considered <span class="tex-font-style-it">valid</span> iff the product of all numbers written on the cards in his new deck is divisible by <span class="tex-span"><i>k</i></span>. So Vova received a deck (possibly not a <span class="tex-font-style-it">valid</span> one) and a number <span class="tex-span"><i>k</i></span>, and now he wonders, how many ways are there to choose <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> so the deck he will get after removing <span class="tex-span"><i>x</i></span> cards from the top and <span class="tex-span"><i>y</i></span> cards from the bottom is <span class="tex-font-style-it">valid</span>?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers written on the cards.</p></div><div class="output-specification"><p>Print the number of ways to choose <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> so the resulting deck is <span class="tex-font-style-it">valid</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers written on the cards.</p>

## Output

<p>Print the number of ways to choose <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> so the resulting deck is <span class="tex-font-style-it">valid</span>.</p>





```input1
3 4
6 2 8

```




```input2
3 6
9 1 14

```




```output1
4

```




```output2
1

```



## Note

<p>In the first example the possible values of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are:</p><ol> <li> <span class="tex-span"><i>x</i> = 0, <i>y</i> = 0</span>; </li><li> <span class="tex-span"><i>x</i> = 1, <i>y</i> = 0</span>; </li><li> <span class="tex-span"><i>x</i> = 2, <i>y</i> = 0</span>; </li><li> <span class="tex-span"><i>x</i> = 0, <i>y</i> = 1</span>. </li></ol>
