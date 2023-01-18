## Description

<div><p>There are $n$ cities in the country. </p><p>Two candidates are fighting for the post of the President. The elections are set in the future, and both candidates have already planned how they are going to connect the cities with roads. Both plans will connect all cities using $n - 1$ roads only. That is, each plan can be viewed as a tree. Both of the candidates had also specified their choice of the capital among $n$ cities ($x$ for the first candidate and $y$ for the second candidate), which may or may not be same.</p><p>Each city has a potential of building a port (one city can have at most one port). Building a port in $i$-th city brings $a_i$ amount of money. However, each candidate has his specific demands. The demands are of the form: </p><ul> <li> $k$ $x$, which means that the candidate wants to build exactly $x$ ports in the subtree of the $k$-th city of his tree (the tree is rooted at the capital of his choice). </li></ul><p>Find out the maximum revenue that can be gained while fulfilling all demands of both candidates, or print <span class="tex-font-style-tt">-1</span> if it is not possible to do.</p><p>It is additionally guaranteed, that each candidate has specified the port demands for the capital of his choice.</p></div><div class="input-specification"><p>The first line contains integers $n$, $x$ and $y$ ($1 \le n \le 500$, $1 \le x, y \le n$)&nbsp;— the number of cities, the capital of the first candidate and the capital of the second candidate respectively.</p><p>Next line contains integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 100\,000$)&nbsp;— the revenue gained if the port is constructed in the corresponding city.</p><p>Each of the next $n - 1$ lines contains integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \ne v_i$), denoting edges between cities in the tree of the first candidate.</p><p>Each of the next $n - 1$ lines contains integers $u'_i$ and $v'_i$ ($1 \le u'_i, v'_i \le n$, $u'_i \ne v'_i$), denoting edges between cities in the tree of the second candidate.</p><p>Next line contains an integer $q_1$ ($1 \le q_1 \le n$), denoting the number of demands of the first candidate.</p><p>Each of the next $q_1$ lines contains two integers $k$ and $x$ ($1 \le k \le n$, $1 \le x \le n$)&nbsp;— the city number and the number of ports in its subtree.</p><p>Next line contains an integer $q_2$ ($1 \le q_2 \le n$), denoting the number of demands of the second candidate.</p><p>Each of the next $q_2$ lines contain two integers $k$ and $x$ ($1 \le k \le n$, $1 \le x \le n$)&nbsp;— the city number and the number of ports in its subtree.</p><p>It is guaranteed, that given edges correspond to valid trees, each candidate has given demand about each city at most once and that each candidate has specified the port demands for the capital of his choice. That is, the city $x$ is always given in demands of the first candidate and city $y$ is always given in the demands of the second candidate.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the maximum possible revenue that can be gained, while satisfying demands of both candidates, or <span class="tex-font-style-tt">-1</span> if it is not possible to satisfy all of the demands.</p></div>

## Input

<p>The first line contains integers $n$, $x$ and $y$ ($1 \le n \le 500$, $1 \le x, y \le n$)&nbsp;— the number of cities, the capital of the first candidate and the capital of the second candidate respectively.</p><p>Next line contains integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 100\,000$)&nbsp;— the revenue gained if the port is constructed in the corresponding city.</p><p>Each of the next $n - 1$ lines contains integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \ne v_i$), denoting edges between cities in the tree of the first candidate.</p><p>Each of the next $n - 1$ lines contains integers $u'_i$ and $v'_i$ ($1 \le u'_i, v'_i \le n$, $u'_i \ne v'_i$), denoting edges between cities in the tree of the second candidate.</p><p>Next line contains an integer $q_1$ ($1 \le q_1 \le n$), denoting the number of demands of the first candidate.</p><p>Each of the next $q_1$ lines contains two integers $k$ and $x$ ($1 \le k \le n$, $1 \le x \le n$)&nbsp;— the city number and the number of ports in its subtree.</p><p>Next line contains an integer $q_2$ ($1 \le q_2 \le n$), denoting the number of demands of the second candidate.</p><p>Each of the next $q_2$ lines contain two integers $k$ and $x$ ($1 \le k \le n$, $1 \le x \le n$)&nbsp;— the city number and the number of ports in its subtree.</p><p>It is guaranteed, that given edges correspond to valid trees, each candidate has given demand about each city at most once and that each candidate has specified the port demands for the capital of his choice. That is, the city $x$ is always given in demands of the first candidate and city $y$ is always given in the demands of the second candidate.</p>

## Output

<p>Print exactly one integer&nbsp;— the maximum possible revenue that can be gained, while satisfying demands of both candidates, or <span class="tex-font-style-tt">-1</span> if it is not possible to satisfy all of the demands.</p>





```input1
4 1 2
1 2 3 4
1 2
1 3
3 4
1 2
2 3
1 4
2
1 3
4 1
1
2 3

```




```input2
5 1 1
3 99 99 100 2
1 2
1 3
3 4
3 5
1 3
1 2
2 4
2 5
2
1 2
3 1
2
1 2
2 1

```




```input3
4 1 2
1 2 3 4
1 2
1 3
3 4
2 1
2 4
4 3
1
1 4
2
4 1
2 4

```




```output1
9
```




```output2
198
```




```output3
-1
```



## Note

<p>In the first example, it is optimal to build ports in cities $2$, $3$ and $4$, which fulfills all demands of both candidates and gives revenue equal to $2 + 3 + 4 = 9$.</p><p>In the second example, it is optimal to build ports in cities $2$ and $3$, which fulfills all demands of both candidates and gives revenue equal to $99 + 99 = 198$. </p><p>In the third example, it is not possible to build ports in such way, that all demands of both candidates are specified, hence the answer is <span class="tex-font-style-tt">-1</span>.</p>
