## Description

<div><p>Two bored soldiers are playing card war. Their card deck consists of exactly <span class="tex-span"><i>n</i></span> cards, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, <span class="tex-font-style-bf">all values are different</span>. They divide cards between them in some manner, it's possible that they have different number of cards. Then they play a "war"-like card game. </p><p>The rules are following. On each turn a <span class="tex-font-style-it">fight</span> happens. Each of them picks card from the top of his stack and puts on the table. The one whose card value is bigger wins this <span class="tex-font-style-it">fight</span> and takes both cards from the table to the bottom of his stack. More precisely, he first takes his opponent's card and puts to the bottom of his stack, and then he puts his card to the bottom of his stack. If after some turn one of the player's stack becomes empty, he loses and the other one wins. </p><p>You have to calculate how many <span class="tex-font-style-it">fights</span> will happen and who will win the game, or state that game won't end.</p></div><div class="input-specification"><p>First line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10</span>), the number of cards.</p><p>Second line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index">1</sub> ≤ <i>n</i> - 1</span>), the number of the first soldier's cards. Then follow <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> integers that are the values on the first soldier's cards, from top to bottom of his stack.</p><p>Third line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>k</i><sub class="lower-index">1</sub> + <i>k</i><sub class="lower-index">2</sub> = <i>n</i></span>), the number of the second soldier's cards. Then follow <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> integers that are the values on the second soldier's cards, from top to bottom of his stack.</p><p><span class="tex-font-style-bf">All card values are different.</span></p></div><div class="output-specification"><p>If somebody wins in this game, print <span class="tex-span">2</span> integers where the first one stands for the number of <span class="tex-font-style-it">fights</span> before end of game and the second one is <span class="tex-span">1</span> or <span class="tex-span">2</span> showing which player has won.</p><p>If the game won't end and will continue forever output <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>First line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10</span>), the number of cards.</p><p>Second line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index">1</sub> ≤ <i>n</i> - 1</span>), the number of the first soldier's cards. Then follow <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> integers that are the values on the first soldier's cards, from top to bottom of his stack.</p><p>Third line contains integer <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>k</i><sub class="lower-index">1</sub> + <i>k</i><sub class="lower-index">2</sub> = <i>n</i></span>), the number of the second soldier's cards. Then follow <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> integers that are the values on the second soldier's cards, from top to bottom of his stack.</p><p><span class="tex-font-style-bf">All card values are different.</span></p>

## Output

<p>If somebody wins in this game, print <span class="tex-span">2</span> integers where the first one stands for the number of <span class="tex-font-style-it">fights</span> before end of game and the second one is <span class="tex-span">1</span> or <span class="tex-span">2</span> showing which player has won.</p><p>If the game won't end and will continue forever output <span class="tex-span"> - 1</span>.</p>





```input1
4
2 1 3
2 4 2

```




```input2
3
1 2
2 1 3

```




```output1
6 2
```




```output2
-1
```



## Note

<p>First sample: </p><center> <img class="tex-graphics" src="file://3KIB8K5i.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Second sample: </p><center> <img class="tex-graphics" src="file://ZQASJdHc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
