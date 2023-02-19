## Description

<div><p><span class="tex-font-style-it">This is an interactive problem</span>.</p><p>Anya has gathered $n$ chess experts numbered from $1$ to $n$ for which the following properties hold:</p><ul> <li> For any pair of players one of the players wins every game against the other (and no draws ever occur); </li><li> Transitivity does not necessarily hold&nbsp;— it might happen that $A$ always beats $B$, $B$ always beats $C$ and $C$ always beats $A$. </li></ul> Anya <span class="tex-font-style-bf">does not</span> know, for each pair, who is the player who beats the other.<p>To organize a tournament, Anya hosts $n-1$ games. In each game, she chooses two players. One of them wins and stays, while the other one is disqualified. After all the games are hosted only one player will remain. A player is said to be a <span class="tex-font-style-it">candidate master</span> if they can win a tournament (notice that the winner of a tournament may depend on the players selected by Anya in the $n-1$ games).</p><p>Since Anya is a curious girl, she is interested in finding the <span class="tex-font-style-it">candidate masters</span>. Unfortunately, she does not have much time. To speed up the process, she will organize up to $2n$ simuls (short for "simultaneous exhibition", in which one player plays against many).</p><p>In one simul, Anya chooses <span class="tex-font-style-bf">exactly one</span> player who will play against some (at least one) of the other players. The chosen player wins all games they would win in a regular game, and the same holds for losses. After the simul finishes, Anya is only told the total number of games won by the chosen player (but not which ones). Nobody is disqualified during a simul.</p><p>Can you help Anya host simuls and determine the <span class="tex-font-style-it">candidate masters</span>?</p><p>The winning players in each pair <span class="tex-font-style-bf">could be</span> changed between the simuls, but only in a way that preserves the results of all previous simuls. These changes may depend on your queries.</p></div><div><h2>Interaction</h2><p>Firstly, the jury sends one integer $n$ ($3 \leq n \leq 250$) which should be read&nbsp;— the number of players. After that, your program may ask queries or report an answer.</p><p>To ask a query, print "<span class="tex-font-style-tt">?</span> $i \; s_1 s_2 \ldots s_n$" (without quotes), where $i$ is the index of the player who will play against some of the other players in the simul. $s$ is a binary string that denotes the players they play against. $i$ plays against every player $j$ for which $s_j = 1$ holds (and $s_j = 1$ should hold for at least one $1 \leq j \leq n$). Please note that $s_i = 0$ must hold since a player cannot play against themselves, otherwise, the query is considered to be incorrect.</p><p>After this, you should read an integer&nbsp;— the number of games player $i$ has won.</p><p>When you have identified the answer, you must print "<span class="tex-font-style-tt">!</span> $c_1 c_2 \ldots c_n$" (without quotes) and terminate your program. $c$ is a binary string which represents the <span class="tex-font-style-it">candidate masters</span>. Player $i$ is a candidate master if $c_i=1$ holds, otherwise, they are not.</p><p>If you ask more than $2n$ queries or if one of the queries is malformed, the interaction terminates immediately and your program receives verdict <span class="tex-font-style-tt">Wrong Answer</span>.</p><p>After printing a query do not forget to output the end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks are disabled in this problem.</span></p></div>





```input1
3

1

1

1
```




```input2
5

0

3

4
```




```output1
? 1 010

? 2 001

? 3 100

! 111
```




```output2
? 5 10110

? 2 10111

? 1 01111

! 10000
```



## Note

<p>In the first example, the first query describes a simul in which player $1$ plays against player $2$ (and no one else). The answer to the query is $1$, meaning that player $1$ won the only game they played. We can conclude that $1$ beats $2$. Similarly, the second query tells us that $2$ beats $3$ and the third query tells us that $3$ beats $1$. All players are <span class="tex-font-style-it">candidate masters</span> in this case as</p><ul> <li> Player $1$ can win the tournament if $2$ and $3$ play first. $3$ loses and leaves, while $2$ stays. $1$ then plays against $2$ and wins; </li><li> Other players can win in the same fashion. </li></ul><p>In the second example, the third query describes a simul in which player $1$ plays against every other player. The answer to the query is $4$, meaning that they won every game they played. It can be concluded that player $1$ also beats every other player. They can never lose, hence they are the only player who can remain at the end of every possible tournament, and the only possible <span class="tex-font-style-it">candidate master</span>. </p>
