## Description

<div><p>The Fair Nut is going to travel to the Tree Country, in which there are $n$ cities. Most of the land of this country is covered by forest. Furthermore, the local road system forms a tree (connected graph without cycles). Nut wants to rent a car in the city $u$ and go by a simple path to city $v$. He hasn't determined the path, so it's time to do it. Note that chosen path can consist of only one vertex.</p><p>A filling station is located in every city. Because of strange law, Nut can buy only $w_i$ liters of gasoline in the $i$-th city. We can assume, that he has <span class="tex-font-style-bf">infinite money</span>. Each road has a length, and as soon as Nut drives through this road, the amount of gasoline decreases by length. Of course, Nut can't choose a path, which consists of roads, where he runs out of gasoline. He can buy gasoline in <span class="tex-font-style-bf">every</span> visited city, even in <span class="tex-font-style-bf">the first</span> and <span class="tex-font-style-bf">the last</span>.</p><p>He also wants to find the maximum amount of gasoline that he can have at the end of the path. Help him: count it.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 3 \cdot 10^5$)&nbsp;— the number of cities.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($0 \leq w_{i} \leq 10^9$)&nbsp;— the maximum amounts of liters of gasoline that Nut can buy in cities.</p><p>Each of the next $n - 1$ lines describes road and contains three integers $u$, $v$, $c$ ($1 \leq u, v \leq n$, $1 \leq c \leq 10^9$, $u \ne v$), where $u$ and $v$&nbsp;— cities that are connected by this road and $c$&nbsp;— its length.</p><p>It is guaranteed that graph of road connectivity is a tree.</p></div><div class="output-specification"><p>Print one number&nbsp;— the maximum amount of gasoline that he can have at the end of the path.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 3 \cdot 10^5$)&nbsp;— the number of cities.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($0 \leq w_{i} \leq 10^9$)&nbsp;— the maximum amounts of liters of gasoline that Nut can buy in cities.</p><p>Each of the next $n - 1$ lines describes road and contains three integers $u$, $v$, $c$ ($1 \leq u, v \leq n$, $1 \leq c \leq 10^9$, $u \ne v$), where $u$ and $v$&nbsp;— cities that are connected by this road and $c$&nbsp;— its length.</p><p>It is guaranteed that graph of road connectivity is a tree.</p>

## Output

<p>Print one number&nbsp;— the maximum amount of gasoline that he can have at the end of the path.</p>





```input1
3
1 3 3
1 2 2
1 3 2

```




```input2
5
6 3 2 5 0
1 2 10
2 3 3
2 4 1
1 5 1

```




```output1
3

```




```output2
7

```



## Note

<p>The optimal way in the first example is $2 \to 1 \to 3$. </p><center> <img class="tex-graphics" height="151px" src="file://MLeqGuru.png" style="max-width: 100.0%;max-height: 100.0%;" width="151px"> </center><p>The optimal way in the second example is $2 \to 4$. </p><center> <img class="tex-graphics" height="227px" src="file://Noc8UTDB.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> </center>
