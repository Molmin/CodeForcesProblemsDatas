## Description

<div><p>Lately, Mr. Chanek frequently plays the game <span class="tex-font-style-bf">Arena of Greed</span>. As the name implies, the game's goal is to find the greediest of them all, who will then be crowned king of Compfestnesia.</p><p>The game is played by two people taking turns, where Mr. Chanek takes the first turn. Initially, there is a treasure chest containing $N$ gold coins. The game ends if there are no more gold coins in the chest. In each turn, the players can make one of the following moves:</p><ul> <li> Take one gold coin from the chest. </li><li> Take half of the gold coins on the chest. This move is only available if the number of coins in the chest is even. </li></ul><p>Both players will try to maximize the number of coins they have. Mr. Chanek asks your help to find the maximum number of coins he can get at the end of the game if both he and the opponent plays optimally.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ $(1 \le T \le 10^5)$ denotes the number of test cases.</p><p>The next $T$ lines each contain a single integer $N$ $(1 \le N \le 10^{18})$.</p></div><div class="output-specification"><p>$T$ lines, each line is the answer requested by Mr. Chanek.</p></div>

## Input

<p>The first line contains a single integer $T$ $(1 \le T \le 10^5)$ denotes the number of test cases.</p><p>The next $T$ lines each contain a single integer $N$ $(1 \le N \le 10^{18})$.</p>

## Output

<p>$T$ lines, each line is the answer requested by Mr. Chanek.</p>





```input1
2
5
6
```




```output1
2
4
```



## Note

<p>For the first case, the game is as follows: </p><ol> <li> Mr. Chanek takes one coin. </li><li> The opponent takes two coins. </li><li> Mr. Chanek takes one coin. </li><li> The opponent takes one coin. </li></ol><p>For the second case, the game is as follows: </p><ol> <li> Mr. Chanek takes three coins. </li><li> The opponent takes one coin. </li><li> Mr. Chanek takes one coin. </li><li> The opponent takes one coin. </li></ol>
