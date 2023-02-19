## Description

<div><p>You are given an integer array $a_1,\ldots, a_n$, where $1\le a_i \le n$ for all $i$.</p><p>There's a "replace" function $f$ which takes a pair of integers $(l, r)$, where $l \le r$, as input and outputs the pair $$f\big( (l, r) \big)=\left(\min\{a_l,a_{l+1},\ldots,a_r\},\, \max\{a_l,a_{l+1},\ldots,a_r\}\right).$$</p><p>Consider repeated calls of this function. That is, from a starting pair $(l, r)$ we get $f\big((l, r)\big)$, then $f\big(f\big((l, r)\big)\big)$, then $f\big(f\big(f\big((l, r)\big)\big)\big)$, and so on.</p><p>Now you need to answer $q$ queries. For the $i$-th query you have two integers $l_i$ and $r_i$ ($1\le l_i\le r_i\le n$). You must answer the minimum number of times you must apply the "replace" function to the pair $(l_i,r_i)$ to get $(1, n)$, or report that it is impossible.</p></div><div class="input-specification"><p>The first line contains two positive integers $n$, $q$ ($1\le n,q\le 10^5$)&nbsp;— the length of the sequence $a$ and the number of the queries.</p><p>The second line contains $n$ positive integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le n$)&nbsp;— the sequence $a$.</p><p>Each line of the following $q$ lines contains two integers $l_i$, $r_i$ ($1\le l_i\le r_i\le n$)&nbsp;— the queries.</p></div><div class="output-specification"><p>For each query, output the required number of times, or $-1$ if it is impossible.</p></div>

## Input

<p>The first line contains two positive integers $n$, $q$ ($1\le n,q\le 10^5$)&nbsp;— the length of the sequence $a$ and the number of the queries.</p><p>The second line contains $n$ positive integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le n$)&nbsp;— the sequence $a$.</p><p>Each line of the following $q$ lines contains two integers $l_i$, $r_i$ ($1\le l_i\le r_i\le n$)&nbsp;— the queries.</p>

## Output

<p>For each query, output the required number of times, or $-1$ if it is impossible.</p>





```input1
5 6
2 5 4 1 3
4 4
1 5
1 4
3 5
4 5
2 3
```




```input2
6 3
2 3 4 6 1 2
5 6
2 5
2 3
```




```input3
5 3
3 2 2 4 1
2 5
1 3
1 5
```




```output1
-1
0
1
2
3
4
```




```output2
5
1
3
```




```output3
-1
-1
0
```



## Note

<p>In the first example, $n=5$ and $a=[2,5,4,1,3]$.</p><p>For the first query: $(4,4)\to(1,1)\to(2,2)\to(5,5)\to(3,3)\to(4,4)\to\ldots$, so it's impossible to get $(1,5)$.</p><p>For the second query, you already have $(1,5)$.</p><p>For the third query: $(1,4)\to(1,5)$.</p><p>For the fourth query: $(3,5)\to(1,4)\to(1,5)$.</p><p>For the fifth query: $(4,5)\to(1,3)\to(2,5)\to(1,5)$.</p><p>For the sixth query: $(2,3)\to(4,5)\to(1,3)\to(2,5)\to(1,5)$.</p>
