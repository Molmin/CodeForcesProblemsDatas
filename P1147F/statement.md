## Description

<div><p>You are given a complete bipartite graph with $2n$ nodes, with $n$ nodes on each side of the bipartition. Nodes $1$ through $n$ are on one side of the bipartition, and nodes $n+1$ to $2n$ are on the other side. You are also given an $n \times n$ matrix $a$ describing the edge weights. $a_{ij}$ denotes the weight of the edge between nodes $i$ and $j+n$. Each edge has a distinct weight.</p><p>Alice and Bob are playing a game on this graph. First Alice chooses to play as either "increasing" or "decreasing" for herself, and Bob gets the other choice. Then she places a token on any node of the graph. Bob then moves the token along any edge incident to that node. They now take turns playing the following game, with Alice going first.</p><p>The current player must move the token from the current vertex to some adjacent unvisited vertex. Let $w$ be the last weight of the last edge that was traversed. The edge that is traversed must be strictly greater than $w$ if the player is playing as "increasing", otherwise, it must be strictly less. The first player unable to make a move loses.</p><p>You are given $n$ and the edge weights of the graph. You can choose to play as either Alice or Bob, and you will play against the judge. You must win all the games for your answer to be judged correct.</p></div><div><h2>Interaction</h2><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). Description of the test cases follows.</p><p>Each test starts with an integer $n$ ($1 \leq n \leq 50$)&nbsp;— the number of nodes on each side of the bipartition.</p><p>The next $n$ lines contain $n$ integers $a_{ij}$ ($1 \leq a_{ij} \leq n^2$). $a_{ij}$ denotes the weight of the edge between node $i$ and node $j+n$. All $a_{ij}$ will be distinct.</p><p>You first print a string "<span class="tex-font-style-tt">A</span>" or "<span class="tex-font-style-tt">B</span>", denoting which player you want to play ("<span class="tex-font-style-tt">A</span>" for Alice and "<span class="tex-font-style-tt">B</span>" for Bob).</p><p>If playing as Alice, first print either "<span class="tex-font-style-tt">I</span>" or "<span class="tex-font-style-tt">D</span>" (denoting whether you choose "increasing" or "decreasing"). Then, print the node that you wish to start at.</p><p>If playing as Bob, read in a character "<span class="tex-font-style-tt">I</span>" or "<span class="tex-font-style-tt">D</span>" (denoting whether the judge chose "increasing" or "decreasing"), then the node that the judge chooses to start at.</p><p>To make a move, print the index of the node that you wish to go to. To read what move the judge made, read an integer from standard in.</p><p>If the judge responds with $-1$, then that means the judge has determined it has no legal moves (or it may have just given up) and that you won the case. Stop processing this case immediately and start processing the next case.</p><p>If the judge responds with $-2$, that means that the judge has determined that you made an invalid move, so you should exit immediately to avoid getting other verdicts.</p><p>If you are unable to make a move or give up, print $-1$ and then exit immediately. This will give you a <span class="tex-font-style-tt">Wrong answer</span> verdict.</p><p>After printing a move do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hack Format</span></p><p>To hack, use the following format. Note that you can only hack with one test case.</p><p>The first line should contain a single integer $t$ ($t=1$).</p><p>The second line should contain an integer $n$ ($1 \leq n \leq 50$).</p><p>The next $n$ lines should contain $n$ integers each, the $a_{ij}$ ($1 \leq a_{ij} \leq n^2$). $a_{ij}$ denotes the weight of the edge between node $i$ and node $j+n$. All $a_{ij}$ must be distinct.</p><p>The judge will play a uniformly random legal move with this case versus the hacked program. If it has no legal moves left, it will give up and declare the player as the winner.</p></div>





```input1
2
3
3 1 9
2 5 7
6 4 8
6
-1
1
1
I 1
-1
```




```output1
A
D 3
2
B
2
```



## Note

<p>The first example has two test cases. In the first test case, the graph looks like the following.</p><center> <img class="tex-graphics" src="file://hV9sGXOo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the sample output, the player decides to play as Alice and chooses "decreasing" and starting at node $3$. The judge responds by moving to node $6$. After, the player moves to node $2$. At this point, the judge has no more moves (since the weight must "increase"), so it gives up and prints $-1$.</p><p>In the next case, we have two nodes connected by an edge of weight $1$. The player decides to play as Bob. No matter what the judge chooses, the player can move the token to the other node and the judge has no moves so will lose.</p>
