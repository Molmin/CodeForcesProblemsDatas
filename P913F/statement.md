## Description

<div><p>There is a chess tournament in All-Right-City. <span class="tex-span"><i>n</i></span> players were invited to take part in the competition. The tournament is held by the following rules:</p><ol> <li> Initially, each player plays one game with every other player. There are no ties; </li><li> After that, the organizers build a complete directed graph with players as vertices. For every pair of players there is exactly one directed edge between them: the winner of their game is the startpoint of this edge and the loser is the endpoint; </li><li> After that, the organizers build a condensation of this graph. The condensation of this graph is an acyclic complete graph, therefore it has the only Hamiltonian path which consists of strongly connected components of initial graph <span class="tex-span"><i>A</i><sub class="lower-index">1</sub> → <i>A</i><sub class="lower-index">2</sub> → ... → <i>A</i><sub class="lower-index"><i>k</i></sub></span>. </li><li> The players from the first component <span class="tex-span"><i>A</i><sub class="lower-index">1</sub></span> are placed on the first <img align="middle" class="tex-formula" src="file://5JyUuOk5.png" style="max-width: 100.0%;max-height: 100.0%;"> places, the players from the component <span class="tex-span"><i>A</i><sub class="lower-index">2</sub></span> are placed on the next <img align="middle" class="tex-formula" src="file://pS7NOo0e.png" style="max-width: 100.0%;max-height: 100.0%;"> places, and so on. </li><li> To determine exact place of each player in a strongly connected component, all the procedures from 1 to 5 are repeated recursively inside each component, i.e. for every <span class="tex-span"><i>i</i> = 1, 2, ..., <i>k</i></span> players from the component <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> play games with each other again, and so on; </li><li> If a component consists of a single player, then he has no more rivals, his place is already determined and the process stops. </li></ol><p>The players are enumerated with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The enumeration was made using results of a previous tournament. It is known that player <span class="tex-span"><i>i</i></span> wins player <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) with probability <span class="tex-span"><i>p</i></span>.</p><p>You need to help to organize the tournament. Find the expected value of total number of games played by all the players. </p><p>It can be shown that the answer can be represented as <img align="middle" class="tex-formula" src="file://v4bs6THa.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime integers and <img align="middle" class="tex-formula" src="file://ZLQ5fneT.png" style="max-width: 100.0%;max-height: 100.0%;">. Print the value of <span class="tex-span"><i>P</i>·<i>Q</i><sup class="upper-index"> - 1</sup></span> modulo <span class="tex-span">998244353</span>.</p><p>If you are not familiar with any of the terms above, you can read about them <a href="https://en.wikipedia.org/wiki/Strongly_connected_component">here</a>.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of players.</p><p>The second line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ 100</span>)&nbsp;— the numerator and the denominator of fraction <img align="middle" class="tex-formula" src="file://dM6hZOIo.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>In the only line print the expected value of total number of games played by all the players. Print the answer using the format above.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of players.</p><p>The second line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ 100</span>)&nbsp;— the numerator and the denominator of fraction <img align="middle" class="tex-formula" src="file://dM6hZOIo.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>In the only line print the expected value of total number of games played by all the players. Print the answer using the format above.</p>





```input1
3
1 2

```




```input2
3
4 6

```




```input3
4
1 2

```




```output1
4

```




```output2
142606340

```




```output3
598946623

```



## Note

<p>In the first example the expected value is <span class="tex-span">4</span>.</p><p>In the second example the expected value is <img align="middle" class="tex-formula" src="file://k85EMmds.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third example the expected value is <img align="middle" class="tex-formula" src="file://LZpLMahJ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
