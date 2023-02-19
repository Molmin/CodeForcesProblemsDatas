## Description

<div><p>Given a positive integer $k$, two arrays are called $k$-similar if:</p><ul> <li> they are <span class="tex-font-style-bf">strictly increasing</span>; </li><li> they have the same length; </li><li> all their elements are positive integers between $1$ and $k$ (inclusive); </li><li> they differ in <span class="tex-font-style-bf">exactly</span> one position. </li></ul><p>You are given an integer $k$, a <span class="tex-font-style-bf">strictly increasing</span> array $a$ and $q$ queries. For each query, you are given two integers $l_i \leq r_i$. Your task is to find how many arrays $b$ exist, such that $b$ is $k$-similar to array $[a_{l_i},a_{l_i+1}\ldots,a_{r_i}]$. </p></div><div class="input-specification"><p>The first line contains three integers $n$, $q$ and $k$ ($1\leq n, q \leq 10^5$, $n\leq k \leq 10^9$)&nbsp;— the length of array $a$, the number of queries and number $k$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots,a_n$ ($1 \leq a_i \leq k$). This array is strictly increasing &nbsp;— $a_1 &lt; a_2 &lt; \ldots &lt; a_n$.</p><p>Each of the following $q$ lines contains two integers $l_i$, $r_i$ ($1 \leq l_i \leq r_i \leq n$).</p></div><div class="output-specification"><p>Print $q$ lines. The $i$-th of them should contain the answer to the $i$-th query.</p></div>

## Input

<p>The first line contains three integers $n$, $q$ and $k$ ($1\leq n, q \leq 10^5$, $n\leq k \leq 10^9$)&nbsp;— the length of array $a$, the number of queries and number $k$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots,a_n$ ($1 \leq a_i \leq k$). This array is strictly increasing &nbsp;— $a_1 &lt; a_2 &lt; \ldots &lt; a_n$.</p><p>Each of the following $q$ lines contains two integers $l_i$, $r_i$ ($1 \leq l_i \leq r_i \leq n$).</p>

## Output

<p>Print $q$ lines. The $i$-th of them should contain the answer to the $i$-th query.</p>





```input1
4 2 5
1 2 4 5
2 3
3 4
```




```input2
6 5 10
2 4 6 7 8 9
1 4
1 2
3 5
1 6
5 5
```




```output1
4
3
```




```output2
8
9
7
6
9
```



## Note

<p>In the first example:</p><p>In the first query there are $4$ arrays that are $5$-similar to $[2,4]$: $[1,4],[3,4],[2,3],[2,5]$.</p><p>In the second query there are $3$ arrays that are $5$-similar to $[4,5]$: $[1,5],[2,5],[3,5]$.</p>
