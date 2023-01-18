## Description

<div><p>Bessie is planning a vacation! In Cow-lifornia, there are $n$ cities, with $n-1$ bidirectional roads connecting them. It is guaranteed that one can reach any city from any other city. </p><p>Bessie is considering $v$ possible vacation plans, with the $i$-th one consisting of a start city $a_i$ and destination city $b_i$.</p><p>It is known that only $r$ of the cities have rest stops. Bessie gets tired easily, and cannot travel across more than $k$ consecutive roads without resting. In fact, she is so desperate to rest that she may travel through the same city multiple times in order to do so.</p><p>For each of the vacation plans, does there exist a way for Bessie to travel from the starting city to the destination city?</p></div><div class="input-specification"><p>The first line contains three integers $n$, $k$, and $r$ ($2 \le n \le 2 \cdot 10^5$, $1 \le k,r \le n$) &nbsp;— the number of cities, the maximum number of roads Bessie is willing to travel through in a row without resting, and the number of rest stops.</p><p>Each of the following $n-1$ lines contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \neq y_i$), meaning city $x_i$ and city $y_i$ are connected by a road. </p><p>The next line contains $r$ integers separated by spaces &nbsp;— the cities with rest stops. Each city will appear at most once.</p><p>The next line contains $v$ ($1 \le v \le 2 \cdot 10^5$) &nbsp;— the number of vacation plans.</p><p>Each of the following $v$ lines contain two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) &nbsp;— the start and end city of the vacation plan. </p></div><div class="output-specification"><p>If Bessie can reach her destination without traveling across more than $k$ roads without resting for the $i$-th vacation plan, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains three integers $n$, $k$, and $r$ ($2 \le n \le 2 \cdot 10^5$, $1 \le k,r \le n$) &nbsp;— the number of cities, the maximum number of roads Bessie is willing to travel through in a row without resting, and the number of rest stops.</p><p>Each of the following $n-1$ lines contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \neq y_i$), meaning city $x_i$ and city $y_i$ are connected by a road. </p><p>The next line contains $r$ integers separated by spaces &nbsp;— the cities with rest stops. Each city will appear at most once.</p><p>The next line contains $v$ ($1 \le v \le 2 \cdot 10^5$) &nbsp;— the number of vacation plans.</p><p>Each of the following $v$ lines contain two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) &nbsp;— the start and end city of the vacation plan. </p>

## Output

<p>If Bessie can reach her destination without traveling across more than $k$ roads without resting for the $i$-th vacation plan, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
6 2 1
1 2
2 3
2 4
4 5
5 6
2
3
1 3
3 5
3 6
```




```input2
8 3 3
1 2
2 3
3 4
4 5
4 6
6 7
7 8
2 5 8
2
7 1
8 1
```




```output1
YES
YES
NO
```




```output2
YES
NO
```



## Note

<p>The graph for the first example is shown below. The rest stop is denoted by red.</p><p>For the first query, Bessie can visit these cities in order: $1, 2, 3$.</p><p>For the second query, Bessie can visit these cities in order: $3, 2, 4, 5$. </p><p>For the third query, Bessie cannot travel to her destination. For example, if she attempts to travel this way: $3, 2, 4, 5, 6$, she travels on more than $2$ roads without resting.</p><center> <img class="tex-graphics" height="227px" src="file://1cbyGIgh.png" style="max-width: 100.0%;max-height: 100.0%;" width="416px">   </center><p>The graph for the second example is shown below. </p><center> <img class="tex-graphics" height="378px" src="file://w5eey07q.png" style="max-width: 100.0%;max-height: 100.0%;" width="416px">   </center>
