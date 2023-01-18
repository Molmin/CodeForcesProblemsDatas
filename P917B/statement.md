## Description

<div><p>As we all know, Max is the best video game player among her friends. Her friends were so jealous of hers, that they created an actual game just to prove that she's not the best at games. The game is played on a directed acyclic graph (a DAG) with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. There's a character written on each edge, a lowercase English letter.</p><center> <img class="tex-graphics" src="file://C25EermZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Max and Lucas are playing the game. Max goes first, then Lucas, then Max again and so on. Each player has a marble, initially located at some vertex. Each player in his/her turn should move his/her marble along some edge (a player can move the marble from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span> if there's an outgoing edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>). If the player moves his/her marble from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span>, the "character" of that round is the character written on the edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>. There's one additional rule; the ASCII code of character of round <span class="tex-span"><i>i</i></span> should be <span class="tex-font-style-bf">greater than or equal</span> to the ASCII code of character of round <span class="tex-span"><i>i</i> - 1</span> (for <span class="tex-span"><i>i</i> &gt; 1</span>). The rounds are numbered for both players together, i.&nbsp;e. Max goes in odd numbers, Lucas goes in even numbers. The player that can't make a move loses the game. The marbles may be at the same vertex at the same time.</p><p>Since the game could take a while and Lucas and Max have to focus on finding Dart, they don't have time to play. So they asked you, if they both play optimally, who wins the game?</p><p>You have to determine the winner of the game for all initial positions of the marbles.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <img align="middle" class="tex-formula" src="file://MF9P1K9J.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the edges. Each line contains two integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> and a lowercase English letter <span class="tex-span"><i>c</i></span>, meaning there's an edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span> written <span class="tex-span"><i>c</i></span> on it (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>). There's at most one edge between any pair of vertices. It is guaranteed that the graph is acyclic.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, a string of length <span class="tex-span"><i>n</i></span> in each one. The <span class="tex-span"><i>j</i></span>-th character in <span class="tex-span"><i>i</i></span>-th line should be 'A' if Max will win the game in case her marble is initially at vertex <span class="tex-span"><i>i</i></span> and Lucas's marble is initially at vertex <span class="tex-span"><i>j</i></span>, and 'B' otherwise.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <img align="middle" class="tex-formula" src="file://MF9P1K9J.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the edges. Each line contains two integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> and a lowercase English letter <span class="tex-span"><i>c</i></span>, meaning there's an edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span> written <span class="tex-span"><i>c</i></span> on it (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>). There's at most one edge between any pair of vertices. It is guaranteed that the graph is acyclic.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, a string of length <span class="tex-span"><i>n</i></span> in each one. The <span class="tex-span"><i>j</i></span>-th character in <span class="tex-span"><i>i</i></span>-th line should be 'A' if Max will win the game in case her marble is initially at vertex <span class="tex-span"><i>i</i></span> and Lucas's marble is initially at vertex <span class="tex-span"><i>j</i></span>, and 'B' otherwise.</p>





```input1
4 4
1 2 b
1 3 a
2 4 c
3 4 b

```




```input2
5 8
5 3 h
1 2 c
3 1 c
3 2 r
5 1 r
4 3 z
5 4 r
5 2 h

```




```output1
BAAA
ABAA
BBBA
BBBB

```




```output2
BABBB
BBBBB
AABBB
AAABA
AAAAB

```



## Note

<p>Here's the graph in the first sample test case:</p><center> <img class="tex-graphics" src="file://L1jlbPSU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Here's the graph in the second sample test case:</p><center> <img class="tex-graphics" src="file://PjmWeXvb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
