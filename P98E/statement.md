## Description

<div><p>Shrek and the Donkey (as you can guess, they also live in the far away kingdom) decided to play a card game called YAGame. The rules are very simple: initially Shrek holds <span class="tex-span"><i>m</i></span> cards and the Donkey holds <span class="tex-span"><i>n</i></span> cards (the players do not see each other's cards), and one more card lies on the table face down so that both players cannot see it as well. Thus, at the beginning of the game there are overall <span class="tex-span"><i>m</i> + <i>n</i> + 1</span> cards. Besides, the players know which cards the pack of cards consists of and their own cards (but they do not know which card lies on the table and which ones the other player has). The players move in turn and Shrek starts. During a move a player can:</p><ul><li> Try to guess which card is lying on the table. If he guesses correctly, the game ends and he wins. If his guess is wrong, the game also ends but this time the other player wins.</li><li> Name any card from the pack. If the other player has such card, he must show it and put it aside (so that this card is no longer used in the game). If the other player doesn't have such card, he says about that.</li></ul> Recently Donkey started taking some yellow pills and winning over Shrek. Now Shrek wants to evaluate his chances to win if he too starts taking the pills.<p>Help Shrek assuming the pills are good in quality and that both players using them start playing in the optimal manner.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>m</i>, <i>n</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print space-separated probabilities that Shrek wins and Donkey wins correspondingly; the absolute error should not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>m</i>, <i>n</i> ≤ 1000</span>).</p>

## Output

<p>Print space-separated probabilities that Shrek wins and Donkey wins correspondingly; the absolute error should not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
0 3

```




```input2
1 0

```




```input3
1 1

```




```output1
0.25 0.75

```




```output2
1 0

```




```output3
0.5 0.5

```


