## Description

<div><p>You are the organizer of the famous "Zurich Music Festival". There will be $n$ singers who will perform at the festival, identified by the integers $1$, $2$, $\dots$, $n$. You must choose in which order they are going to perform on stage. </p><p>You have $m$ friends and each of them has a set of favourite singers. More precisely, for each $1\le i\le m$, the $i$-th friend likes singers $s_{i,1}, \, s_{i, 2}, \, \dots, \,s_{i, q_i}$.</p><p>A friend of yours is happy if the singers he likes perform consecutively (in an arbitrary order). An ordering of the singers is valid if it makes all your friends happy.</p><p>Compute the number of valid orderings modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1\le n,\,m\le 100$) — the number of singers and the number of friends correspondingly.</p><p>The $i$-th of the next $m$ lines contains the integer $q_i$ ($1\le q_i\le n$) — the number of favorite singers of the $i$-th friend – followed by the $q_i$ integers $s_{i,1}, \, s_{i, 2}, \, \dots, \,s_{i, q_i}$ ($1\le s_{i,1}&lt;s_{i,2}&lt;\cdots&lt;s_{i,q_i}\le n$) — the indexes of his favorite singers.</p></div><div class="output-specification"><p>Print the number of valid orderings of the singers modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1\le n,\,m\le 100$) — the number of singers and the number of friends correspondingly.</p><p>The $i$-th of the next $m$ lines contains the integer $q_i$ ($1\le q_i\le n$) — the number of favorite singers of the $i$-th friend – followed by the $q_i$ integers $s_{i,1}, \, s_{i, 2}, \, \dots, \,s_{i, q_i}$ ($1\le s_{i,1}&lt;s_{i,2}&lt;\cdots&lt;s_{i,q_i}\le n$) — the indexes of his favorite singers.</p>

## Output

<p>Print the number of valid orderings of the singers modulo $998\,244\,353$.</p>





```input1
3 1
2 1 3
```




```input2
5 5
2 1 2
2 2 3
2 3 4
2 4 5
2 1 5
```




```input3
100 1
1 50
```




```input4
5 1
5 1 2 3 4 5
```




```input5
2 5
1 2
1 2
1 2
1 1
1 1
```




```input6
11 4
5 4 5 7 9 11
2 2 10
2 9 11
7 1 2 3 5 8 10 11
```




```output1
4
```




```output2
0
```




```output3
35305197
```




```output4
120
```




```output5
2
```




```output6
384
```



## Note

<p><span class="tex-font-style-bf">Explanation of the first sample:</span> There are $3$ singers and only $1$ friend. The friend likes the two singers $1$ and $3$. Thus, the $4$ valid orderings are: </p><ul> <li> <span class="tex-font-style-tt">1 3 2</span> </li><li> <span class="tex-font-style-tt">2 1 3</span> </li><li> <span class="tex-font-style-tt">2 3 1</span> </li><li> <span class="tex-font-style-tt">3 1 2</span> </li></ul><p><span class="tex-font-style-bf">Explanation of the second sample:</span> There are $5$ singers and $5$ friends. One can show that no ordering is valid.</p><p><span class="tex-font-style-bf">Explanation of the third sample:</span> There are $100$ singers and only $1$ friend. The friend likes only singer $50$, hence all the $100!$ possible orderings are valid.</p><p><span class="tex-font-style-bf">Explanation of the fourth sample:</span> There are $5$ singers and only $1$ friend. The friend likes all the singers, hence all the $5!=120$ possible orderings are valid.</p>
