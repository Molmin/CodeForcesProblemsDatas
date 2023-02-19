## Description

<div><p>Eikooc and Sushi play a game.</p><p>The game is played on a tree having $n$ nodes numbered $1$ to $n$. Recall that a tree having $n$ nodes is an undirected, connected graph with $n-1$ edges.</p><p>They take turns alternately moving a token on the tree. <span class="tex-font-style-bf">Eikooc makes the first move, placing the token</span> on any node of her choice. Sushi makes the next move, followed by Eikooc, followed by Sushi, and so on. In each turn after the first, a player must move the token to a node $u$ such that </p><ul> <li> $u$ is adjacent to the node $v$ the token is currently on </li><li> $u$ has not been visited before </li><li> $u \oplus v \leq min(u, v)$ </li></ul><p>Here $x \oplus y$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> operation on integers $x$ and $y$.</p><p>Both the players play optimally. The player who is unable to make a move loses.</p><p>The following are examples which demonstrate the rules of the game. </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><center> <img class="tex-graphics" src="file://g3LBQR2H.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <span class="tex-font-style-it">Suppose Eikooc starts the game by placing the token at node $4$. Sushi then moves the token to node $6$, which is unvisited and adjacent to $4$. It also holds that $6 \oplus 4 = 2 \leq min(6, 4)$. In the next turn, Eikooc moves the token to node $5$, which is unvisited and adjacent to $6$. It holds that $5 \oplus 6 = 3 \leq min(5, 6)$. Sushi has no more moves to play, so she loses.</span></td><td class="tex-tabular-text-align-left"><center> <img class="tex-graphics" src="file://9YChvj4h.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <span class="tex-font-style-it">Suppose Eikooc starts the game by placing the token at node $3$. Sushi moves the token to node $2$, which is unvisited and adjacent to $3$. It also holds that $3 \oplus 2 = 1 \leq min(3, 2)$. Eikooc cannot move the token to node $6$ since $6 \oplus 2 = 4 \nleq min(6, 2)$. Since Eikooc has no moves to play, she loses.</span></td></tr></tbody></table> </center><p>Before the game begins, Eikooc decides to sneakily relabel the nodes of the tree in her favour. Formally, a relabeling is a permutation $p$ of length $n$ (sequence of $n$ integers wherein each integer from $1$ to $n$ occurs exactly once) where $p_i$ denotes the new numbering of node $i$.</p><p>She wants to maximize the number of nodes she can choose in the first turn which will guarantee her a win. Help Eikooc find any relabeling which will help her do so. </p></div><div class="input-specification"><p>The first line contains a single integer $t~(1 \le t \le 10^5)$ &nbsp;— the number of test cases. The description of each test case is as follows.</p><p>The first line of each test case contains an integer $n~(1 \le n \le 2 \cdot 10^5)$ &nbsp;— the number of nodes in the tree.</p><p>The next $n-1$ lines contain two integers $u$ and $v$ $(1 \le u, v \le n; u \neq v)$ &nbsp;— denoting an edge between nodes $u$ and $v$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print any suitable relabeling &nbsp;— a permutation of length $n$ which maximizes the number of nodes that can be chosen in the first turn that guarantee a win for Eikooc. If there are multiple such relabelings, you may print any of them.</p></div>

## Input

<p>The first line contains a single integer $t~(1 \le t \le 10^5)$ &nbsp;— the number of test cases. The description of each test case is as follows.</p><p>The first line of each test case contains an integer $n~(1 \le n \le 2 \cdot 10^5)$ &nbsp;— the number of nodes in the tree.</p><p>The next $n-1$ lines contain two integers $u$ and $v$ $(1 \le u, v \le n; u \neq v)$ &nbsp;— denoting an edge between nodes $u$ and $v$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print any suitable relabeling &nbsp;— a permutation of length $n$ which maximizes the number of nodes that can be chosen in the first turn that guarantee a win for Eikooc. If there are multiple such relabelings, you may print any of them.</p>





```input1
3
1
2
1 2
3
1 2
1 3
```




```output1
1
2 1
1 2 3
```



## Note

<p>In the first test case, Eikooc has only one choice. Sushi will have no moves to play after Eikooc chooses this node and Eikooc will win.</p><p>In the second test case, $1 \oplus 2 = 3 \nleq min(1, 2)$. Hence, after Eikooc picks either of the nodes, Sushi will have no moves to play and Eikooc will win. Both $\{1, 2\}$ and $\{2, 1\}$ are optimal relabelings.</p>
