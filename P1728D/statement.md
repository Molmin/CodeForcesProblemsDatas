## Description

<div><p>Alice and Bob are playing a game. Initially, they are given a non-empty string $s$, consisting of lowercase Latin letters. The length of the string is even. Each player also has a string of their own, initially empty.</p><p>Alice starts, then they alternate moves. In one move, a player takes either the first or the last letter of the string $s$, removes it from $s$ and <span class="tex-font-style-bf">prepends</span> (adds to the beginning) it to their own string.</p><p>The game ends when the string $s$ becomes empty. The winner is the player with a lexicographically smaller string. If the players' strings are equal, then it's a draw.</p><p>A string $a$ is lexicographically smaller than a string $b$ if there exists such position $i$ that $a_j = b_j$ for all $j &lt; i$ and $a_i &lt; b_i$.</p><p>What is the result of the game if both players play optimally (e. g. both players try to win; if they can't, then try to draw)?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a single line&nbsp;— a non-empty string $s$, consisting of lowercase Latin letters. The length of the string $s$ is even.</p><p>The total length of the strings over all testcases doesn't exceed $2000$.</p></div><div class="output-specification"><p>For each testcase, print the result of the game if both players play optimally. If Alice wins, print "Alice". If Bob wins, print "Bob". If it's a draw, print "Draw".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a single line&nbsp;— a non-empty string $s$, consisting of lowercase Latin letters. The length of the string $s$ is even.</p><p>The total length of the strings over all testcases doesn't exceed $2000$.</p>

## Output

<p>For each testcase, print the result of the game if both players play optimally. If Alice wins, print "Alice". If Bob wins, print "Bob". If it's a draw, print "Draw".</p>





```input1|2
2
forces
abba
```




```output1
Alice
Draw
```



## Note

<p>One of the possible games Alice and Bob can play in the first testcase: </p><ol> <li> Alice picks the first letter in $s$: $s=$"orces", $a=$"f", $b=$""; </li><li> Bob picks the last letter in $s$: $s=$"orce", $a=$"f", $b=$"s"; </li><li> Alice picks the last letter in $s$: $s=$"orc", $a=$"ef", $b=$"s"; </li><li> Bob picks the first letter in $s$: $s=$"rc", $a=$"ef", $b=$"os"; </li><li> Alice picks the last letter in $s$: $s=$"r", $a=$"cef", $b=$"os"; </li><li> Bob picks the remaining letter in $s$: $s=$"", $a=$"cef", $b=$"ros". </li></ol><p>Alice wins because "cef" &lt; "ros". Neither of the players follows any strategy in this particular example game, so it doesn't show that Alice wins if both play optimally.</p>
