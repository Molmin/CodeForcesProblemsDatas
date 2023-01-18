## Description

<div><p>Petya and Vasya arranged a game. The game runs by the following rules. Players have a directed graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. One of the vertices contains a chip. Initially the chip is located at vertex <span class="tex-span"><i>s</i></span>. Players take turns moving the chip along some edge of the graph. Petya goes first. Player who can't move the chip loses. If the game lasts for <span class="tex-span">10<sup class="upper-index">6</sup></span> turns the draw is announced.</p><p>Vasya was performing big laboratory work in "Spelling and parts of speech" at night before the game, so he fell asleep at the very beginning of the game. Petya decided to take the advantage of this situation and make both Petya's and Vasya's moves.</p><p>Your task is to help Petya find out if he can win the game or at least draw a tie.</p></div><div class="input-specification"><p>The first line of input contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>&nbsp;— the number of vertices and the number of edges in the graph (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the information about edges of the graph. <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) contains nonnegative integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— number of vertices such that there is an edge from <span class="tex-span"><i>i</i></span> to these vertices and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>&nbsp;— indices of these vertices (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ <i>i</i></span>).</p><p>It is guaranteed that the total sum of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span"><i>m</i></span>.</p><p>The next line contains index of vertex <span class="tex-span"><i>s</i></span>&nbsp;— the initial position of the chip (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>If Petya can win print «<span class="tex-font-style-tt">Win</span>» in the first line. In the next line print numbers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the sequence of vertices Petya should visit for the winning. Vertex <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> should coincide with <span class="tex-span"><i>s</i></span>. For <span class="tex-span"><i>i</i> = 1... <i>k</i> - 1</span> there should be an edge from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> in the graph. There must be no possible move from vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span>. The sequence should be such that Petya wins the game.</p><p>If Petya can't win but can draw a tie, print «<span class="tex-font-style-tt">Draw</span>» in the only line. Otherwise print «<span class="tex-font-style-tt">Lose</span>».</p></div>

## Input

<p>The first line of input contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>&nbsp;— the number of vertices and the number of edges in the graph (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the information about edges of the graph. <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) contains nonnegative integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— number of vertices such that there is an edge from <span class="tex-span"><i>i</i></span> to these vertices and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>&nbsp;— indices of these vertices (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ <i>i</i></span>).</p><p>It is guaranteed that the total sum of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span"><i>m</i></span>.</p><p>The next line contains index of vertex <span class="tex-span"><i>s</i></span>&nbsp;— the initial position of the chip (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>).</p>

## Output

<p>If Petya can win print «<span class="tex-font-style-tt">Win</span>» in the first line. In the next line print numbers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the sequence of vertices Petya should visit for the winning. Vertex <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> should coincide with <span class="tex-span"><i>s</i></span>. For <span class="tex-span"><i>i</i> = 1... <i>k</i> - 1</span> there should be an edge from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> in the graph. There must be no possible move from vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span>. The sequence should be such that Petya wins the game.</p><p>If Petya can't win but can draw a tie, print «<span class="tex-font-style-tt">Draw</span>» in the only line. Otherwise print «<span class="tex-font-style-tt">Lose</span>».</p>





```input1
5 6
2 2 3
2 4 5
1 4
1 5
0
1

```




```input2
3 2
1 3
1 1
0
2

```




```input3
2 2
1 2
1 1
1

```




```output1
Win
1 2 4 5 

```




```output2
Lose

```




```output3
Draw

```



## Note

<p>In the first example the graph is the following:</p><center> <img class="tex-graphics" src="file://6dm6101R.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially the chip is located at vertex <span class="tex-span">1</span>. In the first move Petya moves the chip to vertex <span class="tex-span">2</span>, after that he moves it to vertex <span class="tex-span">4</span> for Vasya. After that he moves to vertex <span class="tex-span">5</span>. Now it is Vasya's turn and there is no possible move, so Petya wins.</p><p>In the second example the graph is the following:</p><center> <img class="tex-graphics" src="file://SvxINHkV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially the chip is located at vertex <span class="tex-span">2</span>. The only possible Petya's move is to go to vertex <span class="tex-span">1</span>. After that he has to go to <span class="tex-span">3</span> for Vasya. Now it's Petya's turn but he has no possible move, so Petya loses.</p><p>In the third example the graph is the following:</p><center> <img class="tex-graphics" src="file://7P6iiVP2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Petya can't win, but he can move along the cycle, so the players will draw a tie.</p>
