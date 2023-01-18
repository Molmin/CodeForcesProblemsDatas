## Description

<div><p>Ilya plays a card game by the following rules.</p><p>A player has several cards. Each card contains two non-negative integers inscribed, one at the top of the card and one at the bottom. At the beginning of the round the player chooses one of his cards to play it. If the top of the card contains number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and the bottom contains number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, then when the player is playing the card, he gets <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> points and also gets the opportunity to play additional <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> cards. After the playing the card is discarded.</p><p>More formally: let's say that there is a counter of the cards that can be played. At the beginning of the round the counter equals one. When a card is played, the counter decreases by one for the played card and increases by the number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, which is written at the bottom of the card. Then the played card is discarded. If after that the counter is not equal to zero, the player gets the opportunity to play another card from the remaining cards. The round ends when the counter reaches zero or the player runs out of cards.</p><p>Of course, Ilya wants to get as many points as possible. Can you determine the maximum number of points he can score provided that you know his cards?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of cards Ilya has.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two non-negative space-separated integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the numbers, written at the top and the bottom of the <span class="tex-span"><i>i</i></span>-th card correspondingly.</p></div><div class="output-specification"><p>Print the single number — the maximum number of points you can score in one round by the described rules.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of cards Ilya has.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two non-negative space-separated integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the numbers, written at the top and the bottom of the <span class="tex-span"><i>i</i></span>-th card correspondingly.</p>

## Output

<p>Print the single number — the maximum number of points you can score in one round by the described rules.</p>





```input1
2
1 0
2 0

```




```input2
3
1 0
2 0
0 2

```




```output1
2

```




```output2
3

```



## Note

<p>In the first sample none of two cards brings extra moves, so you should play the one that will bring more points.</p><p>In the second sample you should first play the third card that doesn't bring any points but lets you play both remaining cards.</p>
