## Description

<div><p>It's our faculty's 34th anniversary! To celebrate this great event, the Faculty of Computer Science, University of Indonesia (Fasilkom), held CPC - Coloring Pavements Competition. The gist of CPC is two players color the predetermined routes of Fasilkom in Blue and Red. There are $N$ Checkpoints and $M$ undirected predetermined routes. Routes $i$ connects checkpoint $U_i$ and $V_i$, for $(1 \le i \le M)$. It is guaranteed that any pair of checkpoints are connected by using one or more routes.</p><p>The rules of CPC is as follows: </p><ul> <li> Two players play in each round. One player plays as blue, the other plays as red. For simplicity, let's call these players $Blue$ and $Red$. </li><li> $Blue$ will color every route in he walks on blue, $Red$ will color the route he walks on red. Both players start at checkpoint number $1$. Initially, all routes are gray. </li><li> Each phase, from their current checkpoint, $Blue$ and $Red$ select a <span class="tex-font-style-bf">different</span> gray route and moves to the checkpoint on the other end of the route simultaneously. </li><li> The game ends when $Blue$ or $Red$ can no longer move. That is, there is no two distinct gray routes they can choose to continue moving. </li></ul><p>Chaneka is interested in participating. However, she does not want to waste much energy. So, She is only interested in the number of final configurations of the routes after each round. Turns out, counting this is also exhausting, so Chaneka asks you to figure this out!</p><p>Two final configurations are considered different if there is a route $U$ in a different color in the two configurations.</p></div><div class="input-specification"><p>The first line contains two integers $N$ and $M$. $N$ $(2 \le N \le 2 \cdot 10^3)$ denotes the number of checkpoints, $M$ $(1 \le M \le 2 \cdot N)$ denotes the number of routes. It is guaranteed that every checkpoint except checkpoint $1$ has exactly two routes connecting it.</p><p>The next $M$ lines each contains two integers $U_i$ and $V_i$ $(1 \le U_i, V_i \le N, U_i \ne V_i)$, which denotes the checkpoint that route $i$ connects.</p><p>It is guaranteed that for every pair of checkpoints, there exists a path connecting them directly or indirectly using the routes. </p></div><div class="output-specification"><p>Output a single integer which denotes the number of final configurations after each round of CPC modulo $10^9 + 7$</p></div>

## Input

<p>The first line contains two integers $N$ and $M$. $N$ $(2 \le N \le 2 \cdot 10^3)$ denotes the number of checkpoints, $M$ $(1 \le M \le 2 \cdot N)$ denotes the number of routes. It is guaranteed that every checkpoint except checkpoint $1$ has exactly two routes connecting it.</p><p>The next $M$ lines each contains two integers $U_i$ and $V_i$ $(1 \le U_i, V_i \le N, U_i \ne V_i)$, which denotes the checkpoint that route $i$ connects.</p><p>It is guaranteed that for every pair of checkpoints, there exists a path connecting them directly or indirectly using the routes. </p>

## Output

<p>Output a single integer which denotes the number of final configurations after each round of CPC modulo $10^9 + 7$</p>





```input1
5 6
1 2
2 3
3 4
4 1
1 5
5 1
```




```output1
8
```



## Note

<p>Every possible final configuration for the example is listed below:</p><center> <img class="tex-graphics" src="file://T9Sjj5G3.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>The blue-colored numbers give the series of moves $Blue$ took, and the red-colored numbers give the series of moves $Red$ took.</p>
