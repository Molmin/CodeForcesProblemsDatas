## Description

<div><p>Kawasiro Nitori is excellent in engineering. Thus she has been appointed to help maintain trains.</p><p>There are $n$ models of trains, and Nitori's department will only have at most one train of each model at any moment. In the beginning, there are no trains, at each of the following $m$ days, one train will be added, or one train will be removed. When a train of model $i$ is added at day $t$, it works for $x_i$ days (day $t$ inclusive), then it is in maintenance for $y_i$ days, then in work for $x_i$ days again, and so on until it is removed.</p><p>In order to make management easier, Nitori wants you to help her calculate how many trains are in maintenance in each day.</p><p><span class="tex-font-style-bf">On a day a train is removed, it is not counted as in maintenance.</span></p></div><div class="input-specification"><p>The first line contains two integers $n$, $m$ ($1 \le n,m \le 2 \cdot 10^5$).</p><p>The $i$-th of the next $n$ lines contains two integers $x_i,y_i$ ($1 \le x_i,y_i \le 10^9$).</p><p>Each of the next $m$ lines contains two integers $op$, $k$ ($1 \le k \le n$, $op = 1$ or $op = 2$). If $op=1$, it means this day's a train of model $k$ is added, otherwise the train of model $k$ is removed. It is guaranteed that when a train of model $x$ is added, there is no train of the same model in the department, and when a train of model $x$ is removed, there is such a train in the department.</p></div><div class="output-specification"><p>Print $m$ lines, The $i$-th of these lines contains one integers, denoting the number of trains in maintenance in the $i$-th day.</p></div>

## Input

<p>The first line contains two integers $n$, $m$ ($1 \le n,m \le 2 \cdot 10^5$).</p><p>The $i$-th of the next $n$ lines contains two integers $x_i,y_i$ ($1 \le x_i,y_i \le 10^9$).</p><p>Each of the next $m$ lines contains two integers $op$, $k$ ($1 \le k \le n$, $op = 1$ or $op = 2$). If $op=1$, it means this day's a train of model $k$ is added, otherwise the train of model $k$ is removed. It is guaranteed that when a train of model $x$ is added, there is no train of the same model in the department, and when a train of model $x$ is removed, there is such a train in the department.</p>

## Output

<p>Print $m$ lines, The $i$-th of these lines contains one integers, denoting the number of trains in maintenance in the $i$-th day.</p>





```input1
3 4
10 15
12 10
1 1
1 3
1 1
2 1
2 3
```




```input2
5 4
1 1
10000000 100000000
998244353 1
2 1
1 2
1 5
2 5
1 5
1 1
```




```output1
0
1
0
0
```




```output2
0
0
0
1
```



## Note

<p>Consider the first example:</p><p>The first day: Nitori adds a train of model $3$. Only a train of model $3$ is running and no train is in maintenance.</p><p>The second day: Nitori adds a train of model $1$. A train of model $1$ is running and a train of model $3$ is in maintenance.</p><p>The third day: Nitori removes a train of model $1$. The situation is the same as the first day.</p><p>The fourth day: Nitori removes a train of model $3$. There are no trains at all.</p>
