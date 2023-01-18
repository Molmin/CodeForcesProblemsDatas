## Description

<div><p>There are $n$ cities in the Kingdom of Autumn, numbered from $1$ to $n$. People can travel between any two cities using $n-1$ two-directional roads.</p><p>This year, the government decides to separate the kingdom. There will be regions of different levels. The whole kingdom will be the region of level $1$. Each region of $i$-th level should be separated into several (at least two) regions of $i+1$-th level, unless $i$-th level is the last level. Each city should belong to exactly one region of each level and for any two cities in the same region, it should be possible to travel between them passing the cities in the same region only.</p><p>According to research, for each city $i$, there is a value $a_i$, which describes the importance of this city. All regions of the same level should have an equal sum of city importances.</p><p>Your task is to find how many plans there are to determine the separation of the regions that all the conditions are satisfied. Two plans are considered different if and only if their numbers of levels are different or there exist two cities in the same region of one level in one plan but in different regions of this level in the other plan. Since the answer may be very large, output it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^6$) — the number of the cities.</p><p>The second line contains $n$ integers, the $i$-th of which is $a_i$ ($1 \leq a_i \leq 10^9$) — the value of each city.</p><p>The third line contains $n-1$ integers, $p_1, p_2, \ldots, p_{n-1}$; $p_i$ ($p_i \leq i$) describes a road between cities $p_i$ and $i+1$.</p></div><div class="output-specification"><p>Print one integer — the number of different plans modulo $10^9+7$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^6$) — the number of the cities.</p><p>The second line contains $n$ integers, the $i$-th of which is $a_i$ ($1 \leq a_i \leq 10^9$) — the value of each city.</p><p>The third line contains $n-1$ integers, $p_1, p_2, \ldots, p_{n-1}$; $p_i$ ($p_i \leq i$) describes a road between cities $p_i$ and $i+1$.</p>

## Output

<p>Print one integer — the number of different plans modulo $10^9+7$.</p>





```input1
4
1 1 1 1
1 2 3

```




```input2
4
1 1 1 1
1 2 2

```




```input3
4
1 2 1 2
1 1 3

```




```output1
4
```




```output2
2
```




```output3
3
```



## Note

<p>For the first example, there are $4$ different plans:</p><p>Plan $1$: Level-$1$: $\{1,2,3,4\}$.</p><p>Plan $2$: Level-$1$: $\{1,2,3,4\}$, Level-$2$: $\{1,2\}$,$\{3,4\}$.</p><p>Plan $3$: Level-$1$: $\{1,2,3,4\}$, Level-$2$: $\{1\}$,$\{2\}$,$\{3\}$,$\{4\}$.</p><p>Plan $4$: Level-$1$: $\{1,2,3,4\}$, Level-$2$: $\{1,2\}$,$\{3,4\}$, Level-$3$: $\{1\}$,$\{2\}$,$\{3\}$,$\{4\}$.</p><p>For the second example, there are $2$ different plans:</p><p>Plan $1$: Level-$1$: $\{1,2,3,4\}$.</p><p>Plan $2$: Level-$1$: $\{1,2,3,4\}$, Level-$2$: $\{1\}$,$\{2\}$,$\{3\}$,$\{4\}$.</p><p>For the third example, there are $3$ different plans:</p><p>Plan $1$: Level-$1$: $\{1,2,3,4\}$.</p><p>Plan $2$: Level-$1$: $\{1,2,3,4\}$, Level-$2$: $\{1,2\}$,$\{3,4\}$.</p><p>Plan $3$: Level-$1$: $\{1,2,3,4\}$, Level-$2$: $\{1,3\}$,$\{2\}$,$\{4\}$.</p>
