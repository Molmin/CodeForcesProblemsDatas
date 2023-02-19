## Description

<div><p>Pak Chanek is playing one of his favourite board games. In the game, there is a directed graph with $N$ vertices and $M$ edges. In the graph, edge $i$ connects two different vertices $U_i$ and $V_i$ with a length of $W_i$. By using the $i$-th edge, something can move from $U_i$ to $V_i$, but not from $V_i$ to $U_i$.</p><p>To play this game, initially Pak Chanek must place both of his hands onto two different vertices. In one move, he can move one of his hands to another vertex using an edge. To move a hand from vertex $U_i$ to vertex $V_i$, Pak Chanek needs a time of $W_i$ seconds. Note that Pak Chanek can only move one hand at a time. This game ends when both of Pak Chanek's hands are on the same vertex.</p><p>Pak Chanek has several questions. For each $p$ satisfying $2 \leq p \leq N$, you need to find the minimum time in seconds needed for Pak Chanek to end the game if initially Pak Chanek's left hand and right hand are placed on vertex $1$ and vertex $p$, or report if it is impossible.</p></div><div class="input-specification"><p>The first line contains two integers $N$ and $M$ ($2 \leq N \leq 10^5$, $0 \leq M \leq 2 \cdot 10^5$) — the number of vertices and edges in the graph.</p><p>The $i$-th of the next $M$ lines contains three integers $U_i$, $V_i$, and $W_i$ ($1 \le U_i, V_i \le N$, $U_i \neq V_i$, $1 \le W_i \le 10^9$) — a directed edge that connects two different vertices $U_i$ and $V_i$ with a length of $W_i$. There is no pair of different edges $i$ and $j$ such that $U_i = U_j$ and $V_i = V_j$.</p></div><div class="output-specification"><p>Output a line containing $N-1$ integers. The $j$-th integer represents the minimum time in seconds needed by Pak Chanek to end the game if initially Pak Chanek's left hand and right hand are placed on vertex $1$ and vertex $j+1$, or $-1$ if it is impossible.</p></div>

## Input

<p>The first line contains two integers $N$ and $M$ ($2 \leq N \leq 10^5$, $0 \leq M \leq 2 \cdot 10^5$) — the number of vertices and edges in the graph.</p><p>The $i$-th of the next $M$ lines contains three integers $U_i$, $V_i$, and $W_i$ ($1 \le U_i, V_i \le N$, $U_i \neq V_i$, $1 \le W_i \le 10^9$) — a directed edge that connects two different vertices $U_i$ and $V_i$ with a length of $W_i$. There is no pair of different edges $i$ and $j$ such that $U_i = U_j$ and $V_i = V_j$.</p>

## Output

<p>Output a line containing $N-1$ integers. The $j$-th integer represents the minimum time in seconds needed by Pak Chanek to end the game if initially Pak Chanek's left hand and right hand are placed on vertex $1$ and vertex $j+1$, or $-1$ if it is impossible.</p>





```input1
5 7
1 2 2
2 4 1
4 1 4
2 5 3
5 4 1
5 2 4
2 1 1
```




```output1
1 -1 3 4
```



## Note

<p>If initially Pak Chanek's left hand is on vertex $1$ and his right hand is on vertex $5$, Pak Chanek can do the following moves: </p><ol> <li> Move his right hand to vertex $4$ in $1$ second. </li><li> Move his left hand to vertex $2$ in $2$ seconds. </li><li> Move his left hand to vertex $4$ in $1$ second. </li></ol><p><img class="tex-graphics" src="file://kGmKgfr6.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In total it needs $1+2+1=4$ seconds. It can be proven that there is no other way that is faster.</p>
