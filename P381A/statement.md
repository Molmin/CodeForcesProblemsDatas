## Description

<div><p>Sereja and Dima play a game. The rules of the game are very simple. The players have <span class="tex-span"><i>n</i></span> cards in a row. Each card contains a number, all numbers on the cards are distinct. The players take turns, Sereja moves first. During his turn a player can take one card: either the leftmost card in a row, or the rightmost one. The game ends when there is no more cards. The player who has the maximum sum of numbers on his cards by the end of the game, wins.</p><p>Sereja and Dima are being greedy. Each of them chooses the card with the larger number during his move.</p><p>Inna is a friend of Sereja and Dima. She knows which strategy the guys are using, so she wants to determine the final score, given the initial state of the game. Help her.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the number of cards on the table. The second line contains space-separated numbers on the cards from left to right. The numbers on the cards are distinct integers from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>On a single line, print two integers. The first number is the number of Sereja's points at the end of the game, the second number is the number of Dima's points at the end of the game.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the number of cards on the table. The second line contains space-separated numbers on the cards from left to right. The numbers on the cards are distinct integers from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p>

## Output

<p>On a single line, print two integers. The first number is the number of Sereja's points at the end of the game, the second number is the number of Dima's points at the end of the game.</p>





```input1
4
4 1 2 10

```




```input2
7
1 2 3 4 5 6 7

```




```output1
12 5

```




```output2
16 12

```



## Note

<p>In the first sample Sereja will take cards with numbers <span class="tex-span">10</span> and <span class="tex-span">2</span>, so Sereja's sum is <span class="tex-span">12</span>. Dima will take cards with numbers <span class="tex-span">4</span> and <span class="tex-span">1</span>, so Dima's sum is <span class="tex-span">5</span>.</p>
