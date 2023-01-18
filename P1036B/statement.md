## Description

<div><p>Mikhail walks on a Cartesian plane. He starts at the point $(0, 0)$, and in one move he can go to any of eight adjacent points. For example, if Mikhail is currently at the point $(0, 0)$, he can go to any of the following points in one move: </p><ul> <li> $(1, 0)$; </li><li> $(1, 1)$; </li><li> $(0, 1)$; </li><li> $(-1, 1)$; </li><li> $(-1, 0)$; </li><li> $(-1, -1)$; </li><li> $(0, -1)$; </li><li> $(1, -1)$. </li></ul><p>If Mikhail goes from the point $(x1, y1)$ to the point $(x2, y2)$ in one move, and $x1 \ne x2$ and $y1 \ne y2$, then such a move is called a <span class="tex-font-style-it">diagonal move</span>.</p><p>Mikhail has $q$ <span class="tex-font-style-bf">queries</span>. For the $i$-th query Mikhail's target is to go to the point $(n_i, m_i)$ from the point $(0, 0)$ in <span class="tex-font-style-bf">exactly</span> $k_i$ moves. Among all possible movements he want to choose one with the maximum number of <span class="tex-font-style-it">diagonal moves</span>. Your task is to find the maximum number of <span class="tex-font-style-it">diagonal moves</span> or find that it is impossible to go from the point $(0, 0)$ to the point $(n_i, m_i)$ in $k_i$ moves.</p><p>Note that Mikhail <span class="tex-font-style-bf">can</span> visit any point any number of times (even the destination point!).</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of queries.</p><p>Then $q$ lines follow. The $i$-th of these $q$ lines contains three integers $n_i$, $m_i$ and $k_i$ ($1 \le n_i, m_i, k_i \le 10^{18}$) — $x$-coordinate of the destination point of the query, $y$-coordinate of the destination point of the query and the number of moves in the query, correspondingly.</p></div><div class="output-specification"><p>Print $q$ integers. The $i$-th integer should be equal to <span class="tex-font-style-tt">-1</span> if Mikhail cannot go from the point $(0, 0)$ to the point $(n_i, m_i)$ in <span class="tex-font-style-bf">exactly</span> $k_i$ moves described above. Otherwise the $i$-th integer should be equal to the the maximum number of <span class="tex-font-style-it">diagonal moves</span> among all possible movements.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of queries.</p><p>Then $q$ lines follow. The $i$-th of these $q$ lines contains three integers $n_i$, $m_i$ and $k_i$ ($1 \le n_i, m_i, k_i \le 10^{18}$) — $x$-coordinate of the destination point of the query, $y$-coordinate of the destination point of the query and the number of moves in the query, correspondingly.</p>

## Output

<p>Print $q$ integers. The $i$-th integer should be equal to <span class="tex-font-style-tt">-1</span> if Mikhail cannot go from the point $(0, 0)$ to the point $(n_i, m_i)$ in <span class="tex-font-style-bf">exactly</span> $k_i$ moves described above. Otherwise the $i$-th integer should be equal to the the maximum number of <span class="tex-font-style-it">diagonal moves</span> among all possible movements.</p>





```input1
3
2 2 3
4 3 7
10 1 9

```




```output1
1
6
-1

```



## Note

<p>One of the possible answers to the first test case: $(0, 0) \to (1, 0) \to (1, 1) \to (2, 2)$.</p><p>One of the possible answers to the second test case: $(0, 0) \to (0, 1) \to (1, 2) \to (0, 3) \to (1, 4) \to (2, 3) \to (3, 2) \to (4, 3)$.</p><p>In the third test case Mikhail cannot reach the point $(10, 1)$ in 9 moves.</p>
