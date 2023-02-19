## Description

<div><p>Alice and Bob are two poachers who cut trees in a forest.</p><p>A forest is a set of zero or more trees. A tree is a connected graph without cycles. A rooted tree has a special vertex called the root. The parent of a node $v$ is the next vertex on the shortest path from $v$ to the root. Children of vertex $v$ are all nodes for which $v$ is the parent. A vertex is a leaf if it has no children.</p><p>In this problem we define the <span class="tex-font-style-it">depth</span> of vertex as number of vertices on the simple path from this vertex to the root. The <span class="tex-font-style-it">rank</span> of a tree is the minimum depth among its leaves.</p><p>Initially there is a forest of rooted trees. Alice and Bob play a game on this forest. They play alternating turns with Alice going first. At the beginning of their turn, the player chooses a tree from the forest. Then the player chooses a positive <span class="tex-font-style-it">cutting depth</span>, which should <span class="tex-font-style-bf">not exceed the rank</span> of the chosen tree. Then the player removes all vertices of that tree whose depth is less that or equal to the cutting depth. All other vertices of the tree form a set of rooted trees with root being the vertex with the smallest depth before the cut. All these trees are included in the game forest and the game continues.</p><p>A player loses if the forest is empty at the beginning of his move.</p><p>You are to determine whether Alice wins the game if both players play optimally.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 5 \cdot 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$) — total number of vertices in the initial forest.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($0 \leq p_i \leq n$) — description of the forest. If $p_i = 0$, then the $i$-th vertex is the root of a tree, otherwise $p_i$ is the parent of the vertex $i$. It's guaranteed that $p$ defines a correct forest of rooted trees.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alice wins, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes). You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 5 \cdot 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$) — total number of vertices in the initial forest.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($0 \leq p_i \leq n$) — description of the forest. If $p_i = 0$, then the $i$-th vertex is the root of a tree, otherwise $p_i$ is the parent of the vertex $i$. It's guaranteed that $p$ defines a correct forest of rooted trees.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alice wins, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes). You can print each letter in any case (upper or lower).</p>





```input1
4
4
0 1 0 3
7
0 1 2 0 4 5 6
4
0 1 1 2
7
0 1 1 2 2 3 3
```




```output1
NO
YES
NO
YES
```



## Note

<p>In the first test case Bob has a symmetric strategy, so Alice cannot win.</p><p><img class="tex-graphics" height="76px" src="file://N7VkHZbA.png" style="max-width: 100.0%;max-height: 100.0%;" width="76px"></p><p>In the second test case Alice can choose the second tree and cutting depth $1$ to get a forest on which she has a symmetric strategy.</p><p><img class="tex-graphics" height="151px" src="file://WuIwAfvZ.png" style="max-width: 100.0%;max-height: 100.0%;" width="76px"></p><p>In third test case the rank of the only tree is $2$ and both possible moves for Alice result in a loss. Bob either can make the forest with a symmetric strategy for himself, or clear the forest.</p><p><img class="tex-graphics" height="151px" src="file://mC5sS5x9.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"></p><p>In the fourth test case all leafs have the same depth, so Alice can clear the forest in one move.</p><p><img class="tex-graphics" height="151px" src="file://mebd3VoO.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"></p>
