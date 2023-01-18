## Description

<div><p>Lately, a national version of a bingo game has become very popular in Berland. There are <span class="tex-span"><i>n</i></span> players playing the game, each player has a card with numbers. The numbers on each card are distinct, but distinct cards can have equal numbers. The card of the <span class="tex-span"><i>i</i></span>-th player contains <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> numbers.</p><p>During the game the host takes numbered balls one by one from a bag. He reads the number aloud in a high and clear voice and then puts the ball away. All participants cross out the number if it occurs on their cards. The person who crosses out all numbers from his card first, wins. If multiple people cross out all numbers from their cards at the same time, there are no winners in the game. At the beginning of the game the bag contains 100 balls numbered 1 through 100, the numbers of all balls are distinct.</p><p>You are given the cards for each player. Write a program that determines whether a player can win the game at the most favorable for him scenario or not.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of the players. Then follow <span class="tex-span"><i>n</i></span> lines, each line describes a player's card. The line that describes a card starts from integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) that shows how many numbers the <span class="tex-span"><i>i</i></span>-th player's card has. Then follows a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>a</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i>, <i>m</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> ≤ 100</span>) — the numbers on the <span class="tex-span"><i>i</i></span>-th player's card. The numbers in the lines are separated by single spaces.</p><p>It is guaranteed that all the numbers on each card are distinct.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain word "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th player can win, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of the players. Then follow <span class="tex-span"><i>n</i></span> lines, each line describes a player's card. The line that describes a card starts from integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) that shows how many numbers the <span class="tex-span"><i>i</i></span>-th player's card has. Then follows a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>a</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i>, <i>m</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> ≤ 100</span>) — the numbers on the <span class="tex-span"><i>i</i></span>-th player's card. The numbers in the lines are separated by single spaces.</p><p>It is guaranteed that all the numbers on each card are distinct.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain word "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the <span class="tex-span"><i>i</i></span>-th player can win, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
3
1 1
3 2 4 1
2 10 11

```




```input2
2
1 1
1 1

```




```output1
YES
NO
YES

```




```output2
NO
NO

```


