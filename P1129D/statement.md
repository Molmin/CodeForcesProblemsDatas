## Description

<div><p>Find the number of ways to divide an array $a$ of $n$ integers into any number of disjoint non-empty segments so that, in each segment, there exist at most $k$ distinct integers that appear exactly once.</p><p>Since the answer can be large, find it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ and $k$ ($1 \leq k \leq n \leq 10^5$) — the number of elements in the array $a$ and the restriction from the statement.</p><p>The following line contains $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$) — elements of the array $a$.</p></div><div class="output-specification"><p>The first and only line contains the number of ways to divide an array $a$ modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two space-separated integers $n$ and $k$ ($1 \leq k \leq n \leq 10^5$) — the number of elements in the array $a$ and the restriction from the statement.</p><p>The following line contains $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$) — elements of the array $a$.</p>

## Output

<p>The first and only line contains the number of ways to divide an array $a$ modulo $998\,244\,353$.</p>





```input1
3 1
1 1 2
```




```input2
5 2
1 1 2 1 3
```




```input3
5 5
1 2 3 4 5
```




```output1
3
```




```output2
14
```




```output3
16
```



## Note

<p>In the first sample, the three possible divisions are as follows.</p><ul> <li> $[[1], [1], [2]]$ </li><li> $[[1, 1], [2]]$ </li><li> $[[1, 1, 2]]$ </li></ul><p>Division $[[1], [1, 2]]$ is not possible because two distinct integers appear exactly once in the second segment $[1, 2]$.</p>
