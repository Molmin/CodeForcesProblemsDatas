## Description

<div><p>"Duel!"</p><p>Betting on the lovely princess Claris, the duel between Tokitsukaze and Quailty has started.</p><p>There are $n$ cards in a row. Each card has two sides, one of which has color. At first, some of these cards are with color sides facing up and others are with color sides facing down. Then they take turns flipping cards, in which Tokitsukaze moves first. In each move, one should choose exactly $k$ consecutive cards and flip them to the same side, which means to make their color sides all face up or all face down. If all the color sides of these $n$ cards face the same direction after one's move, the one who takes this move will win.</p><p>Princess Claris wants to know who will win the game if Tokitsukaze and Quailty are so clever that they won't make mistakes.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$).</p><p>The second line contains a single string of length $n$ that only consists of $0$ and $1$, representing the situation of these $n$ cards, where the color side of the $i$-th card faces up if the $i$-th character is $1$, or otherwise, it faces down and the $i$-th character is $0$.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">once again</span>" (without quotes) if the total number of their moves can exceed $10^9$, which is considered a draw.</p><p>In other cases, print "<span class="tex-font-style-tt">tokitsukaze</span>" (without quotes) if Tokitsukaze will win, or "<span class="tex-font-style-tt">quailty</span>" (without quotes) if Quailty will win.</p><p>Note that the output characters are case-sensitive, and any wrong spelling would be rejected.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$).</p><p>The second line contains a single string of length $n$ that only consists of $0$ and $1$, representing the situation of these $n$ cards, where the color side of the $i$-th card faces up if the $i$-th character is $1$, or otherwise, it faces down and the $i$-th character is $0$.</p>

## Output

<p>Print "<span class="tex-font-style-tt">once again</span>" (without quotes) if the total number of their moves can exceed $10^9$, which is considered a draw.</p><p>In other cases, print "<span class="tex-font-style-tt">tokitsukaze</span>" (without quotes) if Tokitsukaze will win, or "<span class="tex-font-style-tt">quailty</span>" (without quotes) if Quailty will win.</p><p>Note that the output characters are case-sensitive, and any wrong spelling would be rejected.</p>





```input1
4 2
0101
```




```input2
6 1
010101
```




```input3
6 5
010101
```




```input4
4 1
0011
```




```output1
quailty
```




```output2
once again
```




```output3
tokitsukaze
```




```output4
once again
```



## Note

<p>In the first example, no matter how Tokitsukaze moves, there would be three cards with color sides facing the same direction after her move, and Quailty can flip the last card to this direction and win.</p><p>In the second example, no matter how Tokitsukaze moves, Quailty can choose the same card and flip back to the initial situation, which can allow the game to end in a draw.</p><p>In the third example, Tokitsukaze can win by flipping the leftmost five cards up or flipping the rightmost five cards down.</p><p>The fourth example can be explained in the same way as the second example does.</p>
