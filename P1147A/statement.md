## Description

<div><p>Alice and Bob are playing a game on a line with $n$ cells. There are $n$ cells labeled from $1$ through $n$. For each $i$ from $1$ to $n-1$, cells $i$ and $i+1$ are adjacent.</p><p>Alice initially has a token on some cell on the line, and Bob tries to guess where it is. </p><p>Bob guesses a sequence of line cell numbers $x_1, x_2, \ldots, x_k$ in order. In the $i$-th question, Bob asks Alice if her token is currently on cell $x_i$. That is, Alice can answer either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" to each Bob's question.</p><p><span class="tex-font-style-bf">At most one time</span> in this process, before or after answering a question, Alice is allowed to move her token from her current cell to some <span class="tex-font-style-bf">adjacent</span> cell. Alice acted in such a way that she was able to answer "<span class="tex-font-style-tt">NO</span>" to <span class="tex-font-style-bf">all</span> of Bob's questions.</p><p>Note that Alice can even move her token before answering the first question or after answering the last question. Alice can also choose to not move at all.</p><p>You are given $n$ and Bob's questions $x_1, \ldots, x_k$. You would like to count the number of scenarios that let Alice answer "<span class="tex-font-style-tt">NO</span>" to all of Bob's questions. </p><p>Let $(a,b)$ denote a scenario where Alice starts at cell $a$ and ends at cell $b$. Two scenarios $(a_i, b_i)$ and $(a_j, b_j)$ are different if $a_i \neq a_j$ or $b_i \neq b_j$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq n,k \leq 10^5$)&nbsp;— the number of cells and the number of questions Bob asked.</p><p>The second line contains $k$ integers $x_1, x_2, \ldots, x_k$ ($1 \leq x_i \leq n$)&nbsp;— Bob's questions.</p></div><div class="output-specification"><p>Print a single integer, the number of scenarios that let Alice answer "<span class="tex-font-style-tt">NO</span>" to all of Bob's questions.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq n,k \leq 10^5$)&nbsp;— the number of cells and the number of questions Bob asked.</p><p>The second line contains $k$ integers $x_1, x_2, \ldots, x_k$ ($1 \leq x_i \leq n$)&nbsp;— Bob's questions.</p>

## Output

<p>Print a single integer, the number of scenarios that let Alice answer "<span class="tex-font-style-tt">NO</span>" to all of Bob's questions.</p>





```input1
5 3
5 1 4
```




```input2
4 8
1 2 3 4 4 3 2 1
```




```input3
100000 1
42
```




```output1
9
```




```output2
0
```




```output3
299997
```



## Note

<p>The notation $(i,j)$ denotes a scenario where Alice starts at cell $i$ and ends at cell $j$.</p><p>In the first example, the valid scenarios are $(1, 2), (2, 1), (2, 2), (2, 3), (3, 2), (3, 3), (3, 4), (4, 3), (4, 5)$. For example, $(3,4)$ is valid since Alice can start at cell $3$, stay there for the first three questions, then move to cell $4$ after the last question. </p><p>$(4,5)$ is valid since Alice can start at cell $4$, stay there for the first question, the move to cell $5$ for the next two questions. Note that $(4,5)$ is only counted once, even though there are different questions that Alice can choose to do the move, but remember, we only count each pair of starting and ending positions once.</p><p>In the second example, Alice has no valid scenarios.</p><p>In the last example, all $(i,j)$ where $|i-j| \leq 1$ except for $(42, 42)$ are valid scenarios.</p>
