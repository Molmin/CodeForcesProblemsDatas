## Description

<div><p>The government of Berland decided to improve network coverage in his country. Berland has a unique structure: the capital in the center and $n$ cities <span class="tex-font-style-it">in a circle</span> around the capital. The capital already has a good network coverage (so the government ignores it), but the $i$-th city contains $a_i$ households that require a connection.</p><p>The government designed a plan to build $n$ network stations between all pairs of neighboring cities which will maintain connections only for these cities. In other words, the $i$-th network station will provide service only for the $i$-th and the $(i + 1)$-th city (the $n$-th station is connected to the $n$-th and the $1$-st city).</p><p>All network stations have capacities: the $i$-th station can provide the connection to at most $b_i$ households.</p><p>Now the government asks you to check can the designed stations meet the needs of all cities or not — that is, is it possible to assign each household a network station so that each network station $i$ provides the connection to at most $b_i$ households.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($2 \le n \le 10^6$)&nbsp;— the number of cities and stations.</p><p>The second line of each test case contains $n$ integers ($1 \le a_i \le 10^9$)&nbsp;— the number of households in the $i$-th city.</p><p>The third line of each test case contains $n$ integers ($1 \le b_i \le 10^9$)&nbsp;— the capacities of the designed stations.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span>, if the designed stations can meet the needs of all cities, or <span class="tex-font-style-tt">NO</span> otherwise (case insensitive).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($2 \le n \le 10^6$)&nbsp;— the number of cities and stations.</p><p>The second line of each test case contains $n$ integers ($1 \le a_i \le 10^9$)&nbsp;— the number of households in the $i$-th city.</p><p>The third line of each test case contains $n$ integers ($1 \le b_i \le 10^9$)&nbsp;— the capacities of the designed stations.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $10^6$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span>, if the designed stations can meet the needs of all cities, or <span class="tex-font-style-tt">NO</span> otherwise (case insensitive).</p>





```input1
5
3
2 3 4
3 3 3
3
3 3 3
2 3 4
4
2 3 4 5
3 7 2 2
4
4 5 2 3
2 3 2 7
2
1 1
10 10
```




```output1
YES
YES
NO
YES
YES
```



## Note

<p>In the first test case: </p><ul> <li> the first network station can provide $2$ connections to the first city and $1$ connection to the second city; </li><li> the second station can provide $2$ connections to the second city and $1$ connection to the third city; </li><li> the third station can provide $3$ connections to the third city. </li></ul><p>In the second test case: </p><ul> <li> the $1$-st station can provide $2$ connections to the $1$-st city; </li><li> the $2$-nd station can provide $3$ connections to the $2$-nd city; </li><li> the $3$-rd station can provide $3$ connections to the $3$-rd city and $1$ connection to the $1$-st station. </li></ul><p>In the third test case, the fourth city needs $5$ connections, but the third and the fourth station has $4$ connections in total.</p>
