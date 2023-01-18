## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Misha likes to play cooperative games with incomplete information. Today he suggested ten his friends to play a cooperative game "Lake".</p><p>Misha has already come up with a field for the upcoming game. The field for this game is a directed graph consisting of two parts. The first part is a road along the coast of the lake which is a cycle of $c$ vertices. The second part is a path from home to the lake which is a chain of $t$ vertices, and there is an edge from the last vertex of this chain to the vertex of the road along the coast which has the most beautiful view of the lake, also known as the finish vertex. Misha decided to keep the field secret, so nobody knows neither $t$ nor $c$.</p><center> <img class="tex-graphics" height="189px" src="file://V0xuxke8.png" style="max-width: 100.0%;max-height: 100.0%;" width="408px"> </center><p>Note that each vertex of the field has exactly one outgoing edge and all the vertices except the home vertex and the finish vertex have exactly one ingoing edge. The home vertex has no incoming edges, the finish vertex has two incoming edges.</p><p>At the beginning of the game pieces of all the ten players, indexed with consecutive integers from $0$ to $9$, are at the home vertex. After that on each turn some of the players can ask Misha to simultaneously move their pieces along the corresponding edges. Misha will not answer more than $q$ such queries. After each move Misha will tell players whose pieces are at the same vertices and whose pieces are at different vertices.</p><p>The goal of the game is to move all the pieces to the finish vertex. Misha's friends have no idea how to win in such a game without knowledge of $c$, $t$ and $q$, but luckily they are your friends. Help them: coordinate their actions to win the game. </p><p>Misha has drawn such a field that $1 \le t, c$, $(t+c) \leq 1000$ and $q = 3 \cdot (t+c)$.</p></div><div class="input-specification"><p>There is no input&nbsp;— go to the interaction part straight away.</p></div><div class="output-specification"><p>After all friends gather at the finish vertex, print "<span class="tex-font-style-tt">done</span>" and terminate your program.</p></div><div><h2>Interaction</h2><p>To give a command to move the friends, print "<span class="tex-font-style-tt">next</span>" and then space-separated indices of the friends you want to move. For example, to give the command to move the friends with indices $0$, $2$, $5$ and $9$ print "<span class="tex-font-style-tt">next 0 2 5 9</span>". At each turn, you must move at least one of your friends.</p><p>As an answer, first read an integer $k$, and then $10$ digits divided into $k$ space-separated groups. The friends that correspond to the indices in the same group are in the same vertex. The friends that correspond to indices in different groups are in different vertices. The indices in each group follow in ascending order.</p><p>For example, the answer "<span class="tex-font-style-tt">2 05 12346789</span>" means that the friends with indices $0$ and $5$ are in one vertex, and all other friends are in the same but different vertex. The answer "<span class="tex-font-style-tt">4 01 567 234 89</span>" means that Misha's friends are in four different vertices: the friends with indices $0$ and $1$ are in the first, the friends with indices $5$, $6$ and $7$ are in the second, the friends with indices $2$, $3$ and $4$ are in the third, and the friends with indices $8$ and $9$ are in the fourth.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p>Answer "<span class="tex-font-style-tt">stop</span>" instead of a valid one means that you made an invalid query. Exit immediately after receiving "<span class="tex-font-style-tt">stop</span>" and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>In order to hack, print two integers $t$ and $c$ in a single line ($1 \le t, c$, $(t+c) \leq 1000$).</p></div>

## Input

<p>There is no input&nbsp;— go to the interaction part straight away.</p>

## Output

<p>After all friends gather at the finish vertex, print "<span class="tex-font-style-tt">done</span>" and terminate your program.</p>





```input1
2 05 12346789

3 246789 135 0

3 246789 0 135

3 246789 0 135

2 135 0246789

1 0123456789
```




```output1
next 0 5

next 0 1 3

next 2 3 0 1 4 5 6 7 8 9

next 9 8 7 6 5 4 3 2 1 0

next 0 1 3 5

next 1 3 5

done
```



## Note

<p>In the sample input and output values are aligned only for simplicity of interpreting them chronologically. In real interaction no "extra" line breaks should appear.</p><p>In the example, the friends move as follows:</p><center> <img class="tex-graphics" height="287px" src="file://NzdgYMuV.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> </center>
