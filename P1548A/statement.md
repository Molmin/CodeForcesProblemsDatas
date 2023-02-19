## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">When you play the game of thrones, you win, or you die. There is no middle ground.</span></div><div class="epigraph-source">Cersei Lannister, <span class="tex-font-style-it">A Game of Thrones</span> by George R.&nbsp;R. Martin</div></div><p>There are $n$ nobles, numbered from $1$ to $n$. Noble $i$ has a power of $i$. There are also $m$ "friendships". A friendship between nobles $a$ and $b$ is always mutual.</p><p>A noble is defined to be <span class="tex-font-style-it">vulnerable</span> if both of the following conditions are satisfied: </p><ul> <li> the noble has at least one friend, and </li><li> <span class="tex-font-style-bf">all</span> of that noble's friends have a higher power. </li></ul><p>You will have to process the following three types of queries. </p><ol> <li> Add a friendship between nobles $u$ and $v$. </li><li> Remove a friendship between nobles $u$ and $v$. </li><li> Calculate the answer to the following process. </li></ol><p>The process: all vulnerable nobles are simultaneously killed, and all their friendships end. Then, it is possible that new nobles become vulnerable. The process repeats itself until no nobles are vulnerable. It can be proven that the process will end in finite time. After the process is complete, you need to calculate the number of remaining nobles.</p><p>Note that the results of the process are <span class="tex-font-style-bf">not</span> carried over between queries, that is, every process starts with all nobles being alive!</p></div><div class="input-specification"><p>The first line contains the integers $n$ and $m$ ($1 \le n \le 2\cdot 10^5$, $0 \le m \le 2\cdot 10^5$) — the number of nobles and number of original friendships respectively.</p><p>The next $m$ lines each contain the integers $u$ and $v$ ($1 \le u,v \le n$, $u \ne v$), describing a friendship. No friendship is listed twice.</p><p>The next line contains the integer $q$ ($1 \le q \le 2\cdot {10}^{5}$) — the number of queries. </p><p>The next $q$ lines contain the queries themselves, each query has one of the following three formats. </p><ul> <li> $1$ $u$ $v$ ($1 \le u,v \le n$, $u \ne v$) — add a friendship between $u$ and $v$. It is guaranteed that $u$ and $v$ are not friends at this moment. </li><li> $2$ $u$ $v$ ($1 \le u,v \le n$, $u \ne v$) — remove a friendship between $u$ and $v$. It is guaranteed that $u$ and $v$ are friends at this moment. </li><li> $3$ — print the answer to the process described in the statement. </li></ul></div><div class="output-specification"><p>For each type $3$ query print one integer to a new line. It is guaranteed that there will be at least one type $3$ query.</p></div>

## Input

<p>The first line contains the integers $n$ and $m$ ($1 \le n \le 2\cdot 10^5$, $0 \le m \le 2\cdot 10^5$) — the number of nobles and number of original friendships respectively.</p><p>The next $m$ lines each contain the integers $u$ and $v$ ($1 \le u,v \le n$, $u \ne v$), describing a friendship. No friendship is listed twice.</p><p>The next line contains the integer $q$ ($1 \le q \le 2\cdot {10}^{5}$) — the number of queries. </p><p>The next $q$ lines contain the queries themselves, each query has one of the following three formats. </p><ul> <li> $1$ $u$ $v$ ($1 \le u,v \le n$, $u \ne v$) — add a friendship between $u$ and $v$. It is guaranteed that $u$ and $v$ are not friends at this moment. </li><li> $2$ $u$ $v$ ($1 \le u,v \le n$, $u \ne v$) — remove a friendship between $u$ and $v$. It is guaranteed that $u$ and $v$ are friends at this moment. </li><li> $3$ — print the answer to the process described in the statement. </li></ul>

## Output

<p>For each type $3$ query print one integer to a new line. It is guaranteed that there will be at least one type $3$ query.</p>





```input1
4 3
2 1
1 3
3 4
4
3
1 2 3
2 3 1
3
```




```input2
4 3
2 3
3 4
4 1
1
3
```




```output1
2
1
```




```output2
1
```



## Note

<p>Consider the first example. In the first type 3 query, we have the diagram below.</p><p>In the first round of the process, noble $1$ is weaker than all of his friends ($2$ and $3$), and is thus killed. No other noble is vulnerable in round 1. In round 2, noble $3$ is weaker than his only friend, noble $4$, and is therefore killed. At this point, the process ends, and the answer is $2$.</p><center> <img class="tex-graphics" src="file://gHoEqdW6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second type 3 query, the only surviving noble is $4$.</p><p>&nbsp;&nbsp;&nbsp;&nbsp;</p><p>The second example consists of only one type $3$ query. In the first round, two nobles are killed, and in the second round, one noble is killed. The final answer is $1$, since only one noble survives.</p><center> <img class="tex-graphics" src="file://hphxu6K5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
