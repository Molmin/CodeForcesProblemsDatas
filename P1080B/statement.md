## Description

<div><p>Little girl Margarita is a big fan of competitive programming. She especially loves problems about arrays and queries on them.</p><p>Recently, she was presented with an array $a$ of the size of $10^9$ elements that is filled as follows: </p><ul> <li> $a_1 = -1$ </li><li> $a_2 = 2$ </li><li> $a_3 = -3$ </li><li> $a_4 = 4$ </li><li> $a_5 = -5$ </li><li> And so on ... </li></ul><p>That is, the value of the $i$-th element of the array $a$ is calculated using the formula $a_i = i \cdot (-1)^i$.</p><p>She immediately came up with $q$ queries on this array. Each query is described with two numbers: $l$ and $r$. The answer to a query is the sum of all the elements of the array at positions from $l$ to $r$ inclusive.</p><p>Margarita really wants to know the answer to each of the requests. She doesn't want to count all this manually, but unfortunately, she couldn't write the program that solves the problem either. She has turned to you&nbsp;— the best programmer.</p><p>Help her find the answers!</p></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \le q \le 10^3$)&nbsp;— the number of the queries.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le 10^9$)&nbsp;— the descriptions of the queries.</p></div><div class="output-specification"><p>Print $q$ lines, each containing one number&nbsp;— the answer to the query. </p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \le q \le 10^3$)&nbsp;— the number of the queries.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le 10^9$)&nbsp;— the descriptions of the queries.</p>

## Output

<p>Print $q$ lines, each containing one number&nbsp;— the answer to the query. </p>





```input1
5
1 3
2 5
5 5
4 4
2 3
```




```output1
-2
-2
-5
4
-1
```



## Note

<p>In the first query, you need to find the sum of the elements of the array from position $1$ to position $3$. The sum is equal to $a_1 + a_2 + a_3 = -1 + 2 -3 = -2$.</p><p>In the second query, you need to find the sum of the elements of the array from position $2$ to position $5$. The sum is equal to $a_2 + a_3 + a_4 + a_5 = 2 -3 + 4 - 5 = -2$.</p><p>In the third query, you need to find the sum of the elements of the array from position $5$ to position $5$. The sum is equal to $a_5 = -5$.</p><p>In the fourth query, you need to find the sum of the elements of the array from position $4$ to position $4$. The sum is equal to $a_4 = 4$.</p><p>In the fifth query, you need to find the sum of the elements of the array from position $2$ to position $3$. The sum is equal to $a_2 + a_3 = 2 - 3 = -1$.</p>
