## Description

<div><p>Alice and Bob are playing a game on strings.</p><p>Initially, they have some string $t$. In one move the first player selects the character $c$ present in $t$ and erases all it's occurrences in $t$, thus splitting $t$ into many smaller strings. The game then goes independently with each of the strings&nbsp;— to make the move player selects one of the strings and one of the characters there, deletes all occurrences and adds the remaining string back to the game.</p><p>Alice always starts the game, and then Alice and Bob take turns making moves. The player who is unable to make a move (because there is no string left) loses.</p><p>Alice and Bob used to always start with a string $s$, but recently they found out that this became too boring. Now before each game they choose two integers $l$ and $r$ such that $1 \le l \le r \le |s|$ and play the game with the string $s_{l} s_{l+1} s_{l+2} \ldots s_{r}$ instead.</p><p>Given the string $s$ and integers $l$, $r$ for each game. Find who is going to win each game assuming they are smart and are playing optimally.</p></div><div class="input-specification"><p>The first line contains the string $s$ ($1 \le |s| \le 10^5$) consisting of lowercase English letters. This is the string Alice and Bob used to start with.</p><p>The second line contains a single integer $m$ ($1 \le m \le 10^5$)&nbsp;— the number of games to analyze.</p><p>Each of the next $m$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le |s|$)&nbsp;— the bounds of the starting substring in the string $s$.</p></div><div class="output-specification"><p>For each game output a single line containing the name of the winner&nbsp;— "<span class="tex-font-style-tt">Alice</span>" or "<span class="tex-font-style-tt">Bob</span>" respectively.</p></div>

## Input

<p>The first line contains the string $s$ ($1 \le |s| \le 10^5$) consisting of lowercase English letters. This is the string Alice and Bob used to start with.</p><p>The second line contains a single integer $m$ ($1 \le m \le 10^5$)&nbsp;— the number of games to analyze.</p><p>Each of the next $m$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le |s|$)&nbsp;— the bounds of the starting substring in the string $s$.</p>

## Output

<p>For each game output a single line containing the name of the winner&nbsp;— "<span class="tex-font-style-tt">Alice</span>" or "<span class="tex-font-style-tt">Bob</span>" respectively.</p>





```input1
aaab
2
1 2
1 4

```




```input2
aaccbdb
2
5 7
1 7

```




```output1
Alice
Bob

```




```output2
Alice
Alice

```



## Note

<p>In the first example, </p><ol> <li> In the first game the string "<span class="tex-font-style-tt">aa</span>" is selected. Alice deletes character '<span class="tex-font-style-tt">a</span>' and Bob is unable to move. </li><li> In the second game the string "<span class="tex-font-style-tt">aaab</span>" is selected. No matter what character Alice will delete, Bob deletes the other one and Alice is unable to move. </li></ol><p>In the second example Alice wins both game "<span class="tex-font-style-tt">bdb</span>" and "<span class="tex-font-style-tt">aaccbdb</span>".</p><p>To win game "<span class="tex-font-style-tt">bdb</span>" Alice can erase symbol '<span class="tex-font-style-tt">d</span>', the game then goes independently on strings "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">b</span>". Bob deletes one of this strings and the Alice deletes the other one and Bob is unable to move.</p><p>To win game "<span class="tex-font-style-tt">aaccbdb</span>" Alice can erase symbol '<span class="tex-font-style-tt">d</span>', the game then goes independently on strings "<span class="tex-font-style-tt">aaccb</span>" and "<span class="tex-font-style-tt">b</span>". It is possible to show, that no matter what are the moves, the remaining game can only finish in exactly $4$ moves, so the Bob will be unable to move after that.</p>
