## Description

<div><p>After many unsuccessful tries, Mashtali decided to <span class="tex-font-style-striked">copy</span> modify <a href="https://atcoder.jp/contests/agc017/tasks/agc017_d">an AtCoder problem</a>. So here is his <span class="tex-font-style-striked">copied</span> new problem:</p><p>There is a tree with $n$ vertices and some non-empty set of the vertices are pinned to the ground.</p><p>Two players play a game against each other on the tree. They alternately perform the following action:</p><ul> <li> Remove an edge from the tree, then remove every connected component that has no pinned vertex.<p>The player who cannot move loses(every edge has been deleted already). </p></li></ul><p>You are given the tree, but not the set of the pinned vertices. Your task is to determine, for each $k$, the winner of the game, if only the vertices $1, 2, 3, \ldots, k$ are pinned and both players play optimally.</p></div><div class="input-specification"><p>The first line of input contains an integer $n$&nbsp;— the number of vertices ($1 \le n \le 3 \cdot 10^5$).</p><p>The $i$-th of the following $n-1$ lines contains two integers $u_i, v_i$ ($1 \le u_i, v_i \le n$, $u_i \ne v_i$)&nbsp;— the endpoints of the $i$-th edge. It's guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>Print a string of length $n$. The $i$-th character should be '1' if the first player wins the $i$-th scenario, and '2' otherwise.</p></div>

## Input

<p>The first line of input contains an integer $n$&nbsp;— the number of vertices ($1 \le n \le 3 \cdot 10^5$).</p><p>The $i$-th of the following $n-1$ lines contains two integers $u_i, v_i$ ($1 \le u_i, v_i \le n$, $u_i \ne v_i$)&nbsp;— the endpoints of the $i$-th edge. It's guaranteed that these edges form a tree.</p>

## Output

<p>Print a string of length $n$. The $i$-th character should be '1' if the first player wins the $i$-th scenario, and '2' otherwise.</p>





```input1
5
1 2
2 3
2 4
4 5
```




```input2
5
1 2
2 3
1 4
4 5
```




```input3
6
1 2
2 4
5 1
6 3
3 2
```




```input4
7
1 2
3 7
4 6
2 3
2 4
1 5
```




```output1
11122
```




```output2
21122
```




```output3
111111
```




```output4
2212222
```



## Note

<p>Below you can see the tree in the first sample :</p><center> <img class="tex-graphics" src="file://jh9N0CHo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If $k = 1$ then the first player can cut the edge $(1, 2)$.</p><p>If $k = 2$ or $k = 3$, the first player can cut the edge $(2, 4)$, after that only the edges $(1, 2)$ and $(2, 3)$ remain. After the second players move, there will be a single edge left for the first player to cut. So first player wins.</p>
