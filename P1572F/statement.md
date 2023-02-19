## Description

<div><p>There are $n$ cities in a row numbered from $1$ to $n$.</p><p>The cities will be building broadcasting stations. The station in the $i$-th city has height $h_i$ and range $w_i$. It can broadcast information to city $j$ if the following constraints are met: </p><ul> <li> $i \le j \le w_i$, and </li><li> for each $k$ such that $i &lt; k \le j$, the following condition holds: $h_k &lt; h_i$. </li></ul> In other words, the station in city $i$ can broadcast information to city $j$ if $j \ge i$, $j$ is in the range of $i$-th station, and $i$ is strictly highest on the range from $i$ to $j$ (including city $j$).<p>At the beginning, for every city $i$, $h_i = 0$ and $w_i = i$.</p><p>Then $q$ events will take place. During $i$-th event one of the following will happen: </p><ul> <li> City $c_i$ will rebuild its station so that its height will be strictly highest among all stations and $w_{c_i}$ will be set to $g_i$. </li><li> Let $b_j$ be the number of stations that can broadcast information to city $j$. Print the sum of $b_j$ over all $j$ satisfying $l_i \le j \le r_i$. </li></ul><p>Your task is to react to all events and print answers to all queries.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2\cdot10^5$) — number of cities and number of events.</p><p>Then $q$ lines follow. The $i$-th line begins with an integer $p_i$ ($p_i = 1$ or $p_i = 2$).</p><p>If $p_i = 1$ a station will be rebuilt. Then two integers $c_i$ and $g_i$ ($1 \le c_i \le g_i \le n$) follow — the city in which the station is rebuilt and its new broadcasting range.</p><p>If $p_i = 2$ you are given a query. Then two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) follow — the range of cities in the query.</p></div><div class="output-specification"><p>For each query, print in a single line the sum of $b_j$ over the given interval.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2\cdot10^5$) — number of cities and number of events.</p><p>Then $q$ lines follow. The $i$-th line begins with an integer $p_i$ ($p_i = 1$ or $p_i = 2$).</p><p>If $p_i = 1$ a station will be rebuilt. Then two integers $c_i$ and $g_i$ ($1 \le c_i \le g_i \le n$) follow — the city in which the station is rebuilt and its new broadcasting range.</p><p>If $p_i = 2$ you are given a query. Then two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) follow — the range of cities in the query.</p>

## Output

<p>For each query, print in a single line the sum of $b_j$ over the given interval.</p>





```input1
1 3
2 1 1
1 1 1
2 1 1
```




```input2
5 10
1 3 4
2 3 5
1 1 5
2 1 5
1 4 5
2 2 4
1 2 3
2 1 3
1 5 5
2 2 5
```




```output1
1
1
```




```output2
4
10
5
4
5
```



## Note

<p>In the first test case, only station $1$ reaches city $1$ before and after it is rebuilt.</p><p>In the second test case, after each rebuild, the array $b$ looks as follows: </p><ol> <li> $[1, 1, 1, 2, 1]$; </li><li> $[1, 2, 2, 3, 2]$; </li><li> $[1, 2, 2, 1, 2]$; </li><li> $[1, 1, 2, 1, 2]$; </li><li> $[1, 1, 2, 1, 1]$. </li></ol>
