## Description

<div><p>There are $n$ cities in Berland. The city numbered $1$ is the capital. Some pairs of cities are connected by a <span class="tex-font-style-bf">one-way</span> road of length 1.</p><p>Before the trip, Polycarp for each city found out the value of $d_i$&nbsp;— the shortest distance from the capital (the $1$-st city) to the $i$-th city.</p><p>Polycarp begins his journey in the city with number $s$ and, being in the $i$-th city, chooses one of the following actions: </p><ol> <li> Travel from the $i$-th city to the $j$-th city if there is a road from the $i$-th city to the $j$-th and $d_i &lt; d_j$; </li><li> Travel from the $i$-th city to the $j$-th city if there is a road from the $i$-th city to the $j$-th and $d_i \geq d_j$; </li><li> Stop traveling. </li></ol><p>Since the government of Berland does not want all people to come to the capital, so Polycarp <span class="tex-font-style-bf">no more than once</span> can take the second action from the list. in other words, he can perform the second action $0$ or $1$ time during his journey. Polycarp, on the other hand, wants to be as close to the capital as possible.</p><center> <img class="tex-graphics" src="file://1PUmoRjO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For example, if $n = 6$ and the cities are connected, as in the picture above, then Polycarp could have made the following travels (not all possible options): </p><ul> <li> $2 \rightarrow 5 \rightarrow 1 \rightarrow 2 \rightarrow 5$; </li><li> $3 \rightarrow 6 \rightarrow 2$; </li><li> $1 \rightarrow 3 \rightarrow 6 \rightarrow 2 \rightarrow 5$. </li></ul><p>Polycarp wants for each starting city $i$ to find out how close he can get to the capital. More formally: he wants to find the minimal value of $d_j$ that Polycarp can get from the city $i$ to the city $j$ according to the rules described above.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case is preceded by an empty line.</p><p>The first line of each test case contains two integers $n$ ($2 \leq n \leq 2 \cdot 10^5$) and $m$ ($1 \leq m \leq 2 \cdot 10^5$)&nbsp;— number of cities and roads, respectively.</p><p>This is followed by $m$ lines describing the roads. Each road is characterized by two integers $u$ and $v$ ($1 \leq u, v \leq n, u \ne v$)&nbsp;— the numbers of cities connected by a <span class="tex-font-style-bf">one-way</span> road.</p><p>It is guaranteed that the sums of $n$ and $m$ over all test cases do not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that for each pair of different cities $(u, v)$ there is at most one road from $u$ to $v$ (but a pair of roads from $u$ to $v$ and from $v$ to $u$&nbsp;— is valid).</p><p>It is guaranteed that there is a path from the capital to all cities.</p></div><div class="output-specification"><p>For each test case, on a separate line output $n$ numbers, the $i$-th of which is equal to the minimum possible distance from the capital to the city where Polycarp ended his journey.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case is preceded by an empty line.</p><p>The first line of each test case contains two integers $n$ ($2 \leq n \leq 2 \cdot 10^5$) and $m$ ($1 \leq m \leq 2 \cdot 10^5$)&nbsp;— number of cities and roads, respectively.</p><p>This is followed by $m$ lines describing the roads. Each road is characterized by two integers $u$ and $v$ ($1 \leq u, v \leq n, u \ne v$)&nbsp;— the numbers of cities connected by a <span class="tex-font-style-bf">one-way</span> road.</p><p>It is guaranteed that the sums of $n$ and $m$ over all test cases do not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that for each pair of different cities $(u, v)$ there is at most one road from $u$ to $v$ (but a pair of roads from $u$ to $v$ and from $v$ to $u$&nbsp;— is valid).</p><p>It is guaranteed that there is a path from the capital to all cities.</p>

## Output

<p>For each test case, on a separate line output $n$ numbers, the $i$-th of which is equal to the minimum possible distance from the capital to the city where Polycarp ended his journey.</p>





```input1
3

6 7
1 2
1 3
2 5
2 4
5 1
3 6
6 2

2 2
1 2
2 1

6 8
1 2
1 5
2 6
6 1
2 3
3 4
4 2
5 4
```




```output1
0 0 1 2 0 1 
0 0 
0 0 2 1 1 0
```


