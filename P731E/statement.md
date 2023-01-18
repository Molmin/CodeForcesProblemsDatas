## Description

<div><p>Once upon a time Petya and Gena gathered after another programming competition and decided to play some game. As they consider most modern games to be boring, they always try to invent their own games. They have only stickers and markers, but that won't stop them.</p><p>The game they came up with has the following rules. Initially, there are <span class="tex-span"><i>n</i></span> stickers on the wall arranged in a row. Each sticker has some number written on it. Now they alternate turn, Petya moves first.</p><p>One move happens as follows. Lets say there are <span class="tex-span"><i>m</i> ≥ 2</span> stickers on the wall. The player, who makes the current move, picks some integer <span class="tex-span"><i>k</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>m</i></span> and takes <span class="tex-span"><i>k</i></span> leftmost stickers (removes them from the wall). After that he makes the new sticker, puts it to the left end of the row, and writes on it the new integer, equal to the sum of all stickers he took on this move. </p><p>Game ends when there is only one sticker left on the wall. The score of the player is equal to the sum of integers written on all stickers he took during all his moves. The goal of each player is to maximize the difference between his score and the score of his opponent.</p><p>Given the integer <span class="tex-span"><i>n</i></span> and the initial sequence of stickers on the wall, define the result of the game, i.e. the difference between the Petya's and Gena's score if both players play optimally. </p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of stickers, initially located on the wall.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— the numbers on stickers in order from left to right.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the difference between the Petya's score and Gena's score at the end of the game if both players play optimally.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of stickers, initially located on the wall.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— the numbers on stickers in order from left to right.</p>

## Output

<p>Print one integer&nbsp;— the difference between the Petya's score and Gena's score at the end of the game if both players play optimally.</p>





```input1
3
2 4 8

```




```input2
4
1 -7 -2 3

```




```output1
14

```




```output2
-3

```



## Note

<p>In the first sample, the optimal move for Petya is to take all the stickers. As a result, his score will be equal to <span class="tex-span">14</span> and Gena's score will be equal to <span class="tex-span">0</span>.</p><p>In the second sample, the optimal sequence of moves is the following. On the first move Petya will take first three sticker and will put the new sticker with value <span class="tex-span"> - 8</span>. On the second move Gena will take the remaining two stickers. The Petya's score is <span class="tex-span">1 + ( - 7) + ( - 2) =  - 8</span>, Gena's score is <span class="tex-span">( - 8) + 3 =  - 5</span>, i.e. the score difference will be <span class="tex-span"> - 3</span>.</p>
