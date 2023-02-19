## Description

<div><p>$2^n$ people, numbered with distinct integers from $1$ to $2^n$, are playing in a single elimination tournament. The bracket of the tournament is a full binary tree of height $n$ with $2^n$ leaves.</p><p>When two players meet each other in a match, a player with the <span class="tex-font-style-bf">smaller</span> number always wins. The winner of the tournament is the player who wins all $n$ their matches.</p><p>A virtual consolation prize "Wooden Spoon" is awarded to a player who satisfies the following $n$ conditions: </p><ul> <li> they lost their first match; </li><li> the player who beat them lost their second match; </li><li> the player who beat that player lost their third match; </li><li> $\ldots$; </li><li> the player who beat the player from the previous condition lost the final match of the tournament. </li></ul><p>It can be shown that there is always exactly one player who satisfies these conditions.</p><p>Consider all possible $(2^n)!$ arrangements of players into the tournament bracket. For each player, find the number of these arrangements in which they will be awarded the "Wooden Spoon", and print these numbers modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The only line contains a single integer $n$&nbsp;($1 \le n \le 20$)&nbsp;— the size of the tournament.</p><p>There are $20$ tests in the problem: in the first test, $n = 1$; in the second test, $n = 2$; $\ldots$; in the $20$-th test, $n = 20$.</p></div><div class="output-specification"><p>Print $2^n$ integers&nbsp;— the number of arrangements in which the "Wooden Spoon" is awarded to players $1, 2, \ldots, 2^n$, modulo $998\,244\,353$.</p></div>

## Input

<p>The only line contains a single integer $n$&nbsp;($1 \le n \le 20$)&nbsp;— the size of the tournament.</p><p>There are $20$ tests in the problem: in the first test, $n = 1$; in the second test, $n = 2$; $\ldots$; in the $20$-th test, $n = 20$.</p>

## Output

<p>Print $2^n$ integers&nbsp;— the number of arrangements in which the "Wooden Spoon" is awarded to players $1, 2, \ldots, 2^n$, modulo $998\,244\,353$.</p>





```input1
1
```




```input2
2
```




```input3
3
```




```output1
0
2
```




```output2
0
0
8
16
```




```output3
0
0
0
1536
4224
7680
11520
15360
```



## Note

<p>In the first example, the "Wooden Spoon" is always awarded to player $2$.</p><p>In the second example, there are $8$ arrangements where players $1$ and $4$ meet each other in the first match, and in these cases, the "Wooden Spoon" is awarded to player $3$. In the remaining $16$ arrangements, the "Wooden Spoon" is awarded to player $4$.</p>
