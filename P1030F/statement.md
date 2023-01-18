## Description

<div><p>There is an infinite line consisting of cells. There are $n$ boxes in some cells of this line. The $i$-th box stands in the cell $a_i$ and has weight $w_i$. All $a_i$ are distinct, moreover, $a_{i - 1} &lt; a_i$ holds for all valid $i$.</p><p>You would like to put together some boxes. Putting together boxes with <span class="tex-font-style-it">indices</span> in the segment $[l, r]$ means that you will move some of them in such a way that their <span class="tex-font-style-it">positions</span> will form some segment $[x, x + (r - l)]$.</p><p>In one step you can move any box to a neighboring cell if it isn't occupied by another box (i.e. you can choose $i$ and change $a_i$ by $1$, all positions should remain distinct). You spend $w_i$ units of energy moving the box $i$ by one cell. You can move any box any number of times, in arbitrary order.</p><p>Sometimes weights of some boxes change, so you have queries of two types: </p><ol> <li> $id$ $nw$ — weight $w_{id}$ of the box $id$ becomes $nw$. </li><li> $l$ $r$ — you should compute the minimum total energy needed to put together boxes with indices in $[l, r]$. Since the answer can be rather big, print the remainder it gives when divided by $1000\,000\,007 = 10^9 + 7$. Note that the boxes are not moved during the query, you only should compute the answer. </li></ol><p><span class="tex-font-style-bf">Note that you should minimize the answer, not its remainder modulo $10^9 + 7$. So if you have two possible answers $2 \cdot 10^9 + 13$ and $2 \cdot 10^9 + 14$, you should choose the first one and print $10^9 + 6$, even though the remainder of the second answer is $0$.</span></p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the number of boxes and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots a_n$ ($1 \le a_i \le 10^9$) — the positions of the boxes. All $a_i$ are distinct, $a_{i - 1} &lt; a_i$ holds for all valid $i$.</p><p>The third line contains $n$ integers $w_1, w_2, \dots w_n$ ($1 \le w_i \le 10^9$) — the initial weights of the boxes.</p><p>Next $q$ lines describe queries, one query per line.</p><p>Each query is described in a single line, containing two integers $x$ and $y$. If $x &lt; 0$, then this query is of the first type, where $id = -x$, $nw = y$ ($1 \le id \le n$, $1 \le nw \le 10^9$). If $x &gt; 0$, then the query is of the second type, where $l = x$ and $r = y$ ($1 \le l_j \le r_j \le n$). $x$ can not be equal to $0$.</p></div><div class="output-specification"><p>For each query of the second type print the answer on a separate line. Since answer can be large, print the remainder it gives when divided by $1000\,000\,007 = 10^9 + 7$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the number of boxes and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots a_n$ ($1 \le a_i \le 10^9$) — the positions of the boxes. All $a_i$ are distinct, $a_{i - 1} &lt; a_i$ holds for all valid $i$.</p><p>The third line contains $n$ integers $w_1, w_2, \dots w_n$ ($1 \le w_i \le 10^9$) — the initial weights of the boxes.</p><p>Next $q$ lines describe queries, one query per line.</p><p>Each query is described in a single line, containing two integers $x$ and $y$. If $x &lt; 0$, then this query is of the first type, where $id = -x$, $nw = y$ ($1 \le id \le n$, $1 \le nw \le 10^9$). If $x &gt; 0$, then the query is of the second type, where $l = x$ and $r = y$ ($1 \le l_j \le r_j \le n$). $x$ can not be equal to $0$.</p>

## Output

<p>For each query of the second type print the answer on a separate line. Since answer can be large, print the remainder it gives when divided by $1000\,000\,007 = 10^9 + 7$.</p>





```input1
5 8
1 2 6 7 10
1 1 1 1 2
1 1
1 5
1 3
3 5
-3 5
-1 10
1 4
2 5

```




```output1
0
10
3
4
18
7

```



## Note

<p>Let's go through queries of the example: </p><ol> <li> $1\ 1$ — there is only one box so we don't need to move anything. </li><li> $1\ 5$ — we can move boxes to segment $[4, 8]$: $1 \cdot |1 - 4| + 1 \cdot |2 - 5| + 1 \cdot |6 - 6| + 1 \cdot |7 - 7| + 2 \cdot |10 - 8| = 10$. </li><li> $1\ 3$ — we can move boxes to segment $[1, 3]$. </li><li> $3\ 5$ — we can move boxes to segment $[7, 9]$. </li><li> $-3\ 5$ — $w_3$ is changed from $1$ to $5$. </li><li> $-1\ 10$ — $w_1$ is changed from $1$ to $10$. The weights are now equal to $w = [10, 1, 5, 1, 2]$. </li><li> $1\ 4$ — we can move boxes to segment $[1, 4]$. </li><li> $2\ 5$ — we can move boxes to segment $[5, 8]$. </li></ol>
