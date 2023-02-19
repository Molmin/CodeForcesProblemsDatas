## Description

<div><p>There are $n$ cities numbered from $1$ to $n$, and city $i$ has beauty $a_i$.</p><p>A salesman wants to start at city $1$, visit every city exactly once, and return to city $1$.</p><p>For all $i\ne j$, a flight from city $i$ to city $j$ costs $\max(c_i,a_j-a_i)$ dollars, where $c_i$ is the price floor enforced by city $i$. Note that there is no absolute value. Find the minimum total cost for the salesman to complete his trip.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2\le n\le 10^5$) — the number of cities.</p><p>The $i$-th of the next $n$ lines contains two integers $a_i$, $c_i$ ($0\le a_i,c_i\le 10^9$) — the beauty and price floor of the $i$-th city.</p></div><div class="output-specification"><p>Output a single integer — the minimum total cost.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2\le n\le 10^5$) — the number of cities.</p><p>The $i$-th of the next $n$ lines contains two integers $a_i$, $c_i$ ($0\le a_i,c_i\le 10^9$) — the beauty and price floor of the $i$-th city.</p>

## Output

<p>Output a single integer — the minimum total cost.</p>





```input1
3
1 9
2 1
4 1
```




```input2
6
4 2
8 4
3 0
2 3
7 1
0 1
```




```output1
11
```




```output2
13
```



## Note

<p>In the first test case, we can travel in order $1\to 3\to 2\to 1$. </p><ul> <li> The flight $1\to 3$ costs $\max(c_1,a_3-a_1)=\max(9,4-1)=9$. </li><li> The flight $3\to 2$ costs $\max(c_3, a_2-a_3)=\max(1,2-4)=1$. </li><li> The flight $2\to 1$ costs $\max(c_2,a_1-a_2)=\max(1,1-2)=1$. </li></ul><p>The total cost is $11$, and we cannot do better.</p>
