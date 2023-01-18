## Description

<div><p><span class="tex-font-style-it">This is an unusual problem in an unusual contest, here is the announcement: <a href="//codeforces.com/blog/entry/73543">http://codeforces.com/blog/entry/73543</a></span></p><p>You are given an array $A$ of length $n$, initially filled with zeros. You need to process $q$ queries to the array, each of one of the following types: </p><ol> <li> <span class="tex-font-style-tt">1 x y</span>: you need to assign $A_x=y$; </li><li> <span class="tex-font-style-tt">2 l r</span>: you need to print $\sum\limits_{i=l}^r A_i$. </li></ol> Furthermore, there are $T$ independent tests you need to process.</div><div class="input-specification"><p>The first line contains an integer $T$ ($1 \leq T \leq 10^5$) — the number of test cases.</p><p>Each test case description starts with two integers $n, q$ ($1 \leq n, q \leq 10^5$) — the length of the array and the number of queries. The following $q$ lines contain the description of queries: $1~x~y$ ($1 \leq x \leq n$, $0 \leq y \leq 10^9$) for queries of the first type and $2~l~r$ ($1 \leq l \leq r \leq n$) for queries of the second type. </p><p>It is guaranteed that the sum of $n$ as well as the sum of $q$ does not exceed $10^6$.</p></div><div class="output-specification"><p>For each query of the second type print its result on a separate line.</p></div>

## Input

<p>The first line contains an integer $T$ ($1 \leq T \leq 10^5$) — the number of test cases.</p><p>Each test case description starts with two integers $n, q$ ($1 \leq n, q \leq 10^5$) — the length of the array and the number of queries. The following $q$ lines contain the description of queries: $1~x~y$ ($1 \leq x \leq n$, $0 \leq y \leq 10^9$) for queries of the first type and $2~l~r$ ($1 \leq l \leq r \leq n$) for queries of the second type. </p><p>It is guaranteed that the sum of $n$ as well as the sum of $q$ does not exceed $10^6$.</p>

## Output

<p>For each query of the second type print its result on a separate line.</p>





```input1
2
6 5
2 1 6
1 3 2
2 2 4
1 6 3
2 1 6
5 3
1 3 7
1 1 4
2 1 5
```




```output1
0
2
5
11
```


