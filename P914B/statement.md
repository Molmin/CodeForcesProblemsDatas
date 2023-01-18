## Description

<div><p>Edogawa Conan got tired of solving cases, and invited his friend, Professor Agasa, over. They decided to play a game of cards. Conan has <span class="tex-span"><i>n</i></span> cards, and the <span class="tex-span"><i>i</i></span>-th card has a number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> written on it.</p><p>They take turns playing, starting with Conan. In each turn, the player chooses a card and removes it. Also, he removes all cards having a number strictly lesser than the number on the chosen card. Formally, if the player chooses the <span class="tex-span"><i>i</i></span>-th card, he removes that card and removes the <span class="tex-span"><i>j</i></span>-th card for all <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>A player loses if he cannot make a move on his turn, that is, he loses if there are no cards left. Predict the outcome of the game, assuming both players play optimally.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cards Conan has. </p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number on the <span class="tex-span"><i>i</i></span>-th card.</p></div><div class="output-specification"><p>If Conan wins, print "<span class="tex-font-style-tt">Conan</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">Agasa</span>" (without quotes).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cards Conan has. </p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number on the <span class="tex-span"><i>i</i></span>-th card.</p>

## Output

<p>If Conan wins, print "<span class="tex-font-style-tt">Conan</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">Agasa</span>" (without quotes).</p>





```input1
3
4 5 7

```




```input2
2
1 1

```




```output1
Conan

```




```output2
Agasa

```



## Note

<p>In the first example, Conan can just choose the card having number <span class="tex-span">7</span> on it and hence remove all the cards. After that, there are no cards left on Agasa's turn.</p><p>In the second example, no matter which card Conan chooses, there will be one one card left, which Agasa can choose. After that, there are no cards left when it becomes Conan's turn again.</p>
