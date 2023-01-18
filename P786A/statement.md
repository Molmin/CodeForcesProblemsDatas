## Description

<div><p>Rick and Morty are playing their own version of Berzerk (which has nothing in common with the famous Berzerk game). This game needs a huge space, so they play it with a computer.</p><p>In this game there are <span class="tex-span"><i>n</i></span> objects numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> arranged in a circle (in clockwise order). Object number <span class="tex-span">1</span> is a black hole and the others are planets. There's a monster in one of the planet. Rick and Morty don't know on which one yet, only that he's not initially in the black hole, but Unity will inform them before the game starts. But for now, they want to be prepared for every possible scenario.</p><center> <img class="tex-graphics" src="file://WMMVnoRs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Each one of them has a set of numbers between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i> - 1</span> (inclusive). Rick's set is <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> with <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> elements and Morty's is <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> with <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> elements. One of them goes first and the player changes alternatively. In each player's turn, he should choose an arbitrary number like <span class="tex-span"><i>x</i></span> from his set and the monster will move to his <span class="tex-span"><i>x</i></span>-th next object from its current position (clockwise). If after his move the monster gets to the black hole he wins.</p><p>Your task is that for each of monster's initial positions and who plays first determine if the starter wins, loses, or the game will stuck in an infinite loop. In case when player can lose or make game infinity, it more profitable to choose infinity game.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 7000</span>) — number of objects in game.</p><p>The second line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> followed by <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">1, 1</sub>, <i>s</i><sub class="lower-index">1, 2</sub>, ..., <i>s</i><sub class="lower-index">1, <i>k</i><sub class="lower-index">1</sub></sub></span> — Rick's set.</p><p>The third line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> followed by <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">2, 1</sub>, <i>s</i><sub class="lower-index">2, 2</sub>, ..., <i>s</i><sub class="lower-index">2, <i>k</i><sub class="lower-index">2</sub></sub></span> — Morty's set</p><p><span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span> and <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>s</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub> ≤ <i>n</i> - 1</span> for <span class="tex-span">1 ≤ <i>i</i> ≤ 2</span>.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>n</i> - 1</span> words separated by spaces where <span class="tex-span"><i>i</i></span>-th word is "<span class="tex-font-style-tt">Win</span>" (without quotations) if in the scenario that Rick plays first and monster is initially in object number <span class="tex-span"><i>i</i> + 1</span> he wins, "<span class="tex-font-style-tt">Lose</span>" if he loses and "<span class="tex-font-style-tt">Loop</span>" if the game will never end.</p><p>Similarly, in the second line print <span class="tex-span"><i>n</i> - 1</span> words separated by spaces where <span class="tex-span"><i>i</i></span>-th word is "<span class="tex-font-style-tt">Win</span>" (without quotations) if in the scenario that Morty plays first and monster is initially in object number <span class="tex-span"><i>i</i> + 1</span> he wins, "<span class="tex-font-style-tt">Lose</span>" if he loses and "<span class="tex-font-style-tt">Loop</span>" if the game will never end.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 7000</span>) — number of objects in game.</p><p>The second line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> followed by <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">1, 1</sub>, <i>s</i><sub class="lower-index">1, 2</sub>, ..., <i>s</i><sub class="lower-index">1, <i>k</i><sub class="lower-index">1</sub></sub></span> — Rick's set.</p><p>The third line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> followed by <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">2, 1</sub>, <i>s</i><sub class="lower-index">2, 2</sub>, ..., <i>s</i><sub class="lower-index">2, <i>k</i><sub class="lower-index">2</sub></sub></span> — Morty's set</p><p><span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span> and <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>s</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub> ≤ <i>n</i> - 1</span> for <span class="tex-span">1 ≤ <i>i</i> ≤ 2</span>.</p>

## Output

<p>In the first line print <span class="tex-span"><i>n</i> - 1</span> words separated by spaces where <span class="tex-span"><i>i</i></span>-th word is "<span class="tex-font-style-tt">Win</span>" (without quotations) if in the scenario that Rick plays first and monster is initially in object number <span class="tex-span"><i>i</i> + 1</span> he wins, "<span class="tex-font-style-tt">Lose</span>" if he loses and "<span class="tex-font-style-tt">Loop</span>" if the game will never end.</p><p>Similarly, in the second line print <span class="tex-span"><i>n</i> - 1</span> words separated by spaces where <span class="tex-span"><i>i</i></span>-th word is "<span class="tex-font-style-tt">Win</span>" (without quotations) if in the scenario that Morty plays first and monster is initially in object number <span class="tex-span"><i>i</i> + 1</span> he wins, "<span class="tex-font-style-tt">Lose</span>" if he loses and "<span class="tex-font-style-tt">Loop</span>" if the game will never end.</p>





```input1
5
2 3 2
3 1 2 3

```




```input2
8
4 6 2 3 4
2 3 6

```




```output1
Lose Win Win Loop
Loop Win Win Win

```




```output2
Win Win Win Win Win Win Win
Lose Win Lose Lose Win Lose Lose

```


