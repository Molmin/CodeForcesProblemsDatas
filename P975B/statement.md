## Description

<div><p>Mancala is a game famous in the Middle East. It is played on a board that consists of 14 holes. </p><center> <img class="tex-graphics" src="file://mKjLBsuQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially, each hole has $a_i$ stones. When a player makes a move, he chooses a hole which contains a <span class="tex-font-style-bf">positive</span> number of stones. He takes all the stones inside it and then redistributes these stones one by one in the next holes in a counter-clockwise direction.</p><p>Note that the counter-clockwise order means if the player takes the stones from hole $i$, he will put one stone in the $(i+1)$-th hole, then in the $(i+2)$-th, etc. If he puts a stone in the $14$-th hole, the next one will be put in the first hole.</p><p>After the move, the player collects all the stones from holes that contain even number of stones. The number of stones collected by player is the score, according to Resli.</p><p>Resli is a famous Mancala player. He wants to know the maximum score he can obtain after one move.</p></div><div class="input-specification"><p>The only line contains 14 integers $a_1, a_2, \ldots, a_{14}$ ($0 \leq a_i \leq 10^9$)&nbsp;— the number of stones in each hole.</p><p>It is guaranteed that for any $i$ ($1\leq i \leq 14$) $a_i$ is either zero or odd, and there is at least one stone in the board.</p></div><div class="output-specification"><p>Output one integer, the maximum possible score after one move.</p></div>

## Input

<p>The only line contains 14 integers $a_1, a_2, \ldots, a_{14}$ ($0 \leq a_i \leq 10^9$)&nbsp;— the number of stones in each hole.</p><p>It is guaranteed that for any $i$ ($1\leq i \leq 14$) $a_i$ is either zero or odd, and there is at least one stone in the board.</p>

## Output

<p>Output one integer, the maximum possible score after one move.</p>





```input1
0 1 1 0 0 0 0 0 0 7 0 0 0 0

```




```input2
5 1 1 1 1 0 0 0 0 0 0 0 0 0

```




```output1
4

```




```output2
8

```



## Note

<p>In the first test case the board after the move from the hole with $7$ stones will look like <span class="tex-font-style-tt">1 2 2 0 0 0 0 0 0 0 1 1 1 1</span>. Then the player collects the even numbers and ends up with a score equal to $4$.</p>
