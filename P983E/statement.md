## Description

<div><p>In the NN country, there are $n$ cities, numbered from $1$ to $n$, and $n - 1$ roads, connecting them. There is a roads path between any two cities.</p><p>There are $m$ bidirectional bus routes between cities. Buses drive between two cities taking the shortest path with stops in every city they drive through. Travelling by bus, you can travel from any stop on the route to any other. You can travel between cities only by bus.</p><p>You are interested in $q$ questions: is it possible to get from one city to another and what is the minimum number of buses you need to use for it?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of cities.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1 \le p_i &lt; i$), where $p_i$ means that cities $p_i$ and $i$ are connected by road.</p><p>The third line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of bus routes.</p><p>Each of the next $m$ lines contains $2$ integers $a$ and $b$ ($1 \le a, b \le n$, $a \neq b$), meaning that there is a bus route between cities $a$ and $b$. It is possible that there is more than one route between two cities.</p><p>The next line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of questions you are interested in.</p><p>Each of the next $q$ lines contains $2$ integers $v$ and $u$ ($1 \le v, u \le n$, $v \neq u$), meaning that you are interested if it is possible to get from city $v$ to city $u$ and what is the minimum number of buses you need to use for it.</p></div><div class="output-specification"><p>Print the answer for each question on a separate line. If there is no way to get from one city to another, print $-1$. Otherwise print the minimum number of buses you have to use.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of cities.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1 \le p_i &lt; i$), where $p_i$ means that cities $p_i$ and $i$ are connected by road.</p><p>The third line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of bus routes.</p><p>Each of the next $m$ lines contains $2$ integers $a$ and $b$ ($1 \le a, b \le n$, $a \neq b$), meaning that there is a bus route between cities $a$ and $b$. It is possible that there is more than one route between two cities.</p><p>The next line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of questions you are interested in.</p><p>Each of the next $q$ lines contains $2$ integers $v$ and $u$ ($1 \le v, u \le n$, $v \neq u$), meaning that you are interested if it is possible to get from city $v$ to city $u$ and what is the minimum number of buses you need to use for it.</p>

## Output

<p>Print the answer for each question on a separate line. If there is no way to get from one city to another, print $-1$. Otherwise print the minimum number of buses you have to use.</p>





```input1
7
1 1 1 4 5 6
4
4 2
5 4
1 3
6 7
6
4 5
3 5
7 2
4 5
3 2
5 3

```




```input2
7
1 1 2 3 4 1
4
4 7
3 5
7 6
7 6
6
4 6
3 1
3 2
2 7
6 3
5 3

```




```output1
1
3
-1
1
2
3

```




```output2
1
-1
-1
1
-1
1

```



## Note

<center> <img class="tex-graphics" src="file://XEB43Vew.png" style="max-width: 100.0%;max-height: 100.0%;"> Routes for first sample are marked on the picture. </center>
