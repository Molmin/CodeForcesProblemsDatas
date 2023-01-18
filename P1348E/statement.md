## Description

<div><p>Phoenix is picking berries in his backyard. There are $n$ shrubs, and each shrub has $a_i$ red berries and $b_i$ blue berries.</p><p>Each basket can contain $k$ berries. But, Phoenix has decided that each basket may only contain berries from the same shrub or berries of the same color (red or blue). In other words, all berries in a basket must be from the same shrub or/and have the same color.</p><p>For example, if there are two shrubs with $5$ red and $2$ blue berries in the first shrub and $2$ red and $1$ blue berries in the second shrub then Phoenix can fill $2$ baskets of capacity $4$ completely: </p><ul> <li> the first basket will contain $3$ red and $1$ blue berries from the first shrub; </li><li> the second basket will contain the $2$ remaining red berries from the first shrub and $2$ red berries from the second shrub. </li></ul><p>Help Phoenix determine the maximum number of baskets he can <span class="tex-font-style-bf">fill completely</span>!</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($ 1\le n, k \le 500$)&nbsp;— the number of shrubs and the basket capacity, respectively.</p><p>The $i$-th of the next $n$ lines contain two integers $a_i$ and $b_i$ ($0 \le a_i, b_i \le 10^9$)&nbsp;— the number of red and blue berries in the $i$-th shrub, respectively.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum number of baskets that Phoenix can fill completely.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($ 1\le n, k \le 500$)&nbsp;— the number of shrubs and the basket capacity, respectively.</p><p>The $i$-th of the next $n$ lines contain two integers $a_i$ and $b_i$ ($0 \le a_i, b_i \le 10^9$)&nbsp;— the number of red and blue berries in the $i$-th shrub, respectively.</p>

## Output

<p>Output one integer&nbsp;— the maximum number of baskets that Phoenix can fill completely.</p>





```input1
2 4
5 2
2 1
```




```input2
1 5
2 3
```




```input3
2 5
2 1
1 3
```




```input4
1 2
1000000000 1
```




```output1
2
```




```output2
1
```




```output3
0
```




```output4
500000000
```



## Note

<p>The first example is described above.</p><p>In the second example, Phoenix can fill one basket fully using all the berries from the first (and only) shrub.</p><p>In the third example, Phoenix cannot fill any basket completely because there are less than $5$ berries in each shrub, less than $5$ total red berries, and less than $5$ total blue berries.</p><p>In the fourth example, Phoenix can put all the red berries into baskets, leaving an extra blue berry behind.</p>
