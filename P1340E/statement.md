## Description

<div><p><span class="tex-font-style-bf">Unfortunately, a mistake was found in the proof of the author's solution to this problem. Currently, we don't know the absolutely correct solution. However, you can solve this task, but if your solution passes all the tests, it is not guaranteed to be correct. If your solution has passed all the tests and you are sure that it is correct, you can write to one of the contest authors about it.</span></p><p><span class="tex-font-style-it"> Surely you all read the book "Alice in Wonderland". In this task, Nastya got to the country of Three strange Bees. The bees are strange because their honeycombs are pentagonal. Nastya got there illegally, so she wants bees not to catch her. Help the bees punish the intruder! </span></p><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>A beehive is a connected undirected graph where bees and Nastya can move along the edges. A graph satisfies two properties: </p><ul> <li> The degree of any of its vertex is no more than $3$. </li><li> For each edge, there exists a cycle of length not greater than $5$ passing through this edge. </li></ul> There are three bees and Nastya. You play for bees. Firstly, you choose the vertices where you put the bees. Then Nastya chooses another vertex in which she will initially appear. One move is first moving the bees, then Nastya, in turn: <ol> <li> For each of your bees, you can either move each one along some edge from the vertex they are currently staying or leave it in place. </li><li> Then Nastya will <span class="tex-font-style-bf">necessarily</span> move along some edge of the graph from the vertex she is currently staying/. </li></ol><p>You win if at least one of the bees and Nastya are in the same vertex at any time of the game.</p><p>If this situation does not occur after $n$ moves, then you lose.</p><p><span class="tex-font-style-bf">Several bees can be in the same vertex.</span></p></div><div class="input-specification"><p>The first line contains two integers $n$ $(4 \leq n \leq 5000)$ and $m$ $(n \leq m \leq 3n)$ &nbsp;— the number of vertices and edges in the graph.</p><p>Each of the next $m$ lines contains two integers $v$ and $u$ $(1 \leq v, u \leq n)$, which mean that there is an edge between the vertices $v$ and $u$. It is guaranteed that the graph is connected, does not contain loops that the degree of any vertex does not exceed $3$ and a cycle of length no more than $5$ passes through each edge. Note that the graph <span class="tex-font-style-bf">may</span> contain multiple edges.</p></div><div><h2>Interaction</h2><p>At each turn, you must output exactly three vertices $a, b, c$ $(1 \leq a, b, c \leq n)$. For the first time, $3$ vertices displayed will indicate which vertices you originally placed bees on. In response, you will receive the vertex where the jury placed Nastya. Each next $3$ vertices will indicate where the $3$ bees move at your turn. Each of the bees can, regardless of other bees, both remain at the current vertex and move along the edge. After the next output of $3$ vertices, in response, you get the number of the new vertex to which Nastya went.</p><p>As soon as one of the bees is at the same vertex with Nastya or you have reached the limit on the number of moves, your program should stop working. That is if you made a move, and one of the bees ended up at the same vertex with Nastya, your program must stop working, or if Nastya made a move and ended up at the same vertex with one of the bees, you should not make your move and the program should stop working.</p><p>If the number of moves exceeds limit ($n$, where $n$ is the number of vertices), you will get the Wrong Answer verdict.</p><p>Your solution may receive the verdict <span class="tex-font-style-it">Idleness Limit Exceeded</span> if you don't output anything or forget to flush the output buffer.</p><p>To flush the output buffer, you need to do the following immediately after printing the query and the line end:</p><ul> <li> fflush(stdout) or cout.flush() in C++; </li><li> System.out.flush() in Java; </li><li> flush(output) in Pascal; </li><li> stdout.flush() in Python; </li><li> for other languages see documentation. </li></ul><p>In this problem interactor is <span class="tex-font-style-bf">adaptive</span>. This means that depending on all your previous moves, Nastya's behavior may change.</p><p><span class="tex-font-style-bf">Hacks</span> are not available for this problem.</p></div>

## Input

<p>The first line contains two integers $n$ $(4 \leq n \leq 5000)$ and $m$ $(n \leq m \leq 3n)$ &nbsp;— the number of vertices and edges in the graph.</p><p>Each of the next $m$ lines contains two integers $v$ and $u$ $(1 \leq v, u \leq n)$, which mean that there is an edge between the vertices $v$ and $u$. It is guaranteed that the graph is connected, does not contain loops that the degree of any vertex does not exceed $3$ and a cycle of length no more than $5$ passes through each edge. Note that the graph <span class="tex-font-style-bf">may</span> contain multiple edges.</p>





```input1
5 5
1 2
2 3
3 4
4 5
5 1
4
5
```




```input2
8 9
1 2
2 3
3 4
4 5
5 1
5 6
6 7
7 8
8 4
1
5
```




```output1
1 1 2
1 5 3
```




```output2
7 3 3
6 2 2
5 3 1
```



## Note

<p>Let Nastya be a green chip, and three numbered red ones are three bees.</p><p>In the first test, the movement of the heroes looks like this.</p><center> <img class="tex-graphics" height="302px" src="file://zuBvAtpe.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">After selecting the starting vertices.</span> </center><center> <img class="tex-graphics" height="302px" src="file://BLWHwc9i.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">The first move after the bees move.</span> </center><center> <img class="tex-graphics" height="302px" src="file://TrYUIOWC.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">The first move after the Nastya's move. The first bee caught Nastya.</span> </center><p>In the second test, the movement of the heroes looks like this.</p><center> <img class="tex-graphics" height="302px" src="file://XnB1WkSV.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">After selecting the starting vertices.</span> </center><center> <img class="tex-graphics" height="302px" src="file://Fidpdq95.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">The first move after the bees move.</span> </center><center> <img class="tex-graphics" height="302px" src="file://UlW5pQ1m.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">The first move after the Nastya's move.</span> </center><center> <img class="tex-graphics" height="302px" src="file://1ik75xHP.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px">   <span class="tex-font-size-small">The second move after the bees move. The first bee caught Nastya.</span> </center>
