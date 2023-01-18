## Description

<div><p>There is a card game called "Durak", which means "Fool" in Russian. The game is quite popular in the countries that used to form USSR. The problem does not state all the game's rules explicitly — you can find them later yourselves if you want.</p><p>To play durak you need a pack of <span class="tex-span">36</span> cards. Each card has a suit ("<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">D</span>" and "<span class="tex-font-style-tt">C</span>") and a rank (in the increasing order "<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>" and "<span class="tex-font-style-tt">A</span>"). At the beginning of the game one suit is arbitrarily chosen as trump. </p><p>The players move like that: one player puts one or several of his cards on the table and the other one should beat each of them with his cards.</p><p>A card beats another one if both cards have similar suits and the first card has a higher rank then the second one. Besides, a trump card can beat any non-trump card whatever the cards’ ranks are. In all other cases you can not beat the second card with the first one.</p><p>You are given the trump suit and two different cards. Determine whether the first one beats the second one or not.</p></div><div class="input-specification"><p>The first line contains the tramp suit. It is "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">D</span>" or "<span class="tex-font-style-tt">C</span>".</p><p>The second line contains the description of the two different cards. Each card is described by one word consisting of two symbols. The first symbol stands for the rank ("<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>" and "<span class="tex-font-style-tt">A</span>"), and the second one stands for the suit ("<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">D</span>" and "<span class="tex-font-style-tt">C</span>").</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the first cards beats the second one. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (also without the quotes).</p></div>

## Input

<p>The first line contains the tramp suit. It is "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">D</span>" or "<span class="tex-font-style-tt">C</span>".</p><p>The second line contains the description of the two different cards. Each card is described by one word consisting of two symbols. The first symbol stands for the rank ("<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>" and "<span class="tex-font-style-tt">A</span>"), and the second one stands for the suit ("<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">D</span>" and "<span class="tex-font-style-tt">C</span>").</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the first cards beats the second one. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (also without the quotes).</p>





```input1
H
QH 9S

```




```input2
S
8D 6D

```




```input3
C
7H AS

```




```output1
YES

```




```output2
YES
```




```output3
NO
```


