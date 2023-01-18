## Description

<div><p>There are $n$ persons who initially don't know each other. On each morning, two of them, who were not friends before, become friends.</p><p>We want to plan a trip for every evening of $m$ days. On each trip, you have to select a group of people that will go on the trip. For every person, one of the following should hold: </p><ul> <li> Either this person does not go on the trip, </li><li> Or at least $k$ of his friends also go on the trip. </li></ul><p>Note that the friendship is not transitive. That is, if $a$ and $b$ are friends and $b$ and $c$ are friends, it does not necessarily imply that $a$ and $c$ are friends.</p><p>For each day, find the maximum number of people that can go on the trip on that day.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $k$ ($2 \leq n \leq 2 \cdot 10^5, 1 \leq m \leq 2 \cdot 10^5$, $1 \le k &lt; n$)&nbsp;— the number of people, the number of days and the number of friends each person on the trip should have in the group.</p><p>The $i$-th ($1 \leq i \leq m$) of the next $m$ lines contains two integers $x$ and $y$ ($1\leq x, y\leq n$, $x\ne y$), meaning that persons $x$ and $y$ become friends on the morning of day $i$. It is guaranteed that $x$ and $y$ were not friends before.</p></div><div class="output-specification"><p>Print exactly $m$ lines, where the $i$-th of them ($1\leq i\leq m$) contains the maximum number of people that can go on the trip on the evening of the day $i$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $k$ ($2 \leq n \leq 2 \cdot 10^5, 1 \leq m \leq 2 \cdot 10^5$, $1 \le k &lt; n$)&nbsp;— the number of people, the number of days and the number of friends each person on the trip should have in the group.</p><p>The $i$-th ($1 \leq i \leq m$) of the next $m$ lines contains two integers $x$ and $y$ ($1\leq x, y\leq n$, $x\ne y$), meaning that persons $x$ and $y$ become friends on the morning of day $i$. It is guaranteed that $x$ and $y$ were not friends before.</p>

## Output

<p>Print exactly $m$ lines, where the $i$-th of them ($1\leq i\leq m$) contains the maximum number of people that can go on the trip on the evening of the day $i$.</p>





```input1
4 4 2
2 3
1 2
1 3
1 4

```




```input2
5 8 2
2 1
4 2
5 4
5 2
4 3
5 1
4 1
3 2

```




```input3
5 7 2
1 5
3 2
2 5
3 4
1 2
5 3
1 3

```




```output1
0
0
3
3

```




```output2
0
0
0
3
3
4
4
5

```




```output3
0
0
0
0
3
4
4

```



## Note

<p>In the first example, </p><ul> <li> $1,2,3$ can go on day $3$ and $4$. </li></ul><p>In the second example, </p><ul> <li> $2,4,5$ can go on day $4$ and $5$. </li><li> $1,2,4,5$ can go on day $6$ and $7$. </li><li> $1,2,3,4,5$ can go on day $8$. </li></ul><p>In the third example, </p><ul> <li> $1,2,5$ can go on day $5$. </li><li> $1,2,3,5$ can go on day $6$ and $7$. </li></ul>
