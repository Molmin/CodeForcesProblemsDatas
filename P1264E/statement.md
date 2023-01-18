## Description

<div><p>A football league has recently begun in Beautiful land. There are $n$ teams participating in the league. Let's enumerate them with integers from $1$ to $n$.</p><p>There will be played exactly $\frac{n(n-1)}{2}$ matches: each team will play against all other teams exactly once. In each match, there is always a winner and loser and there is no draw.</p><p>After all matches are played, the organizers will count the number of <span class="tex-font-style-it">beautiful triples</span>. Let's call a triple of three teams $(A, B, C)$ beautiful if a team $A$ win against a team $B$, a team $B$ win against a team $C$ and a team $C$ win against a team $A$. We look only to a triples of different teams and the order of teams in the triple is important.</p><p>The beauty of the league is the number of beautiful triples.</p><p>At the moment, $m$ matches were played and their results are known.</p><p>What is the maximum beauty of the league that can be, after playing all remaining matches? Also find a possible results for all remaining $\frac{n(n-1)}{2} - m$ matches, so that the league has this maximum beauty.</p></div><div class="input-specification"><p>The first line contains two integers $n, m$ ($3 \leq n \leq 50, 0 \leq m \leq \frac{n(n-1)}{2}$)&nbsp;— the number of teams in the football league and the number of matches that were played.</p><p>Each of $m$ following lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n$, $u \neq v$) denoting that the $u$-th team won against the $v$-th team. It is guaranteed that each unordered pair of teams appears at most once.</p></div><div class="output-specification"><p>Print $n$ lines, each line having a string of exactly $n$ characters. Each character must be either $0$ or $1$.</p><p>Let $a_{ij}$ be the $j$-th number in the $i$-th line. For all $1 \leq i \leq n$ it should be true, that $a_{ii} = 0$. For all pairs of teams $i \neq j$ the number $a_{ij}$ indicates the result of the match between the $i$-th team and the $j$-th team:</p><ul> <li> If $a_{ij}$ is $1$, the $i$-th team wins against the $j$-th team; </li><li> Otherwise the $j$-th team wins against the $i$-th team; </li><li> Also, it should be true, that $a_{ij} + a_{ji} = 1$. </li></ul><p>Also note that the results of the $m$ matches that were already played cannot be changed in your league.</p><p>The beauty of the league in the output should be maximum possible. If there are multiple possible answers with maximum beauty, you can print any of them.</p></div>

## Input

<p>The first line contains two integers $n, m$ ($3 \leq n \leq 50, 0 \leq m \leq \frac{n(n-1)}{2}$)&nbsp;— the number of teams in the football league and the number of matches that were played.</p><p>Each of $m$ following lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n$, $u \neq v$) denoting that the $u$-th team won against the $v$-th team. It is guaranteed that each unordered pair of teams appears at most once.</p>

## Output

<p>Print $n$ lines, each line having a string of exactly $n$ characters. Each character must be either $0$ or $1$.</p><p>Let $a_{ij}$ be the $j$-th number in the $i$-th line. For all $1 \leq i \leq n$ it should be true, that $a_{ii} = 0$. For all pairs of teams $i \neq j$ the number $a_{ij}$ indicates the result of the match between the $i$-th team and the $j$-th team:</p><ul> <li> If $a_{ij}$ is $1$, the $i$-th team wins against the $j$-th team; </li><li> Otherwise the $j$-th team wins against the $i$-th team; </li><li> Also, it should be true, that $a_{ij} + a_{ji} = 1$. </li></ul><p>Also note that the results of the $m$ matches that were already played cannot be changed in your league.</p><p>The beauty of the league in the output should be maximum possible. If there are multiple possible answers with maximum beauty, you can print any of them.</p>





```input1
3 1
1 2
```




```input2
4 2
1 2
1 3
```




```output1
010
001
100
```




```output2
0110
0001
0100
1010
```



## Note

<p>The beauty of league in the first test case is equal to $3$ because there exists three beautiful triples: $(1, 2, 3)$, $(2, 3, 1)$, $(3, 1, 2)$.</p><p>The beauty of league in the second test is equal to $6$ because there exists six beautiful triples: $(1, 2, 4)$, $(2, 4, 1)$, $(4, 1, 2)$, $(2, 4, 3)$, $(4, 3, 2)$, $(3, 2, 4)$.</p>
