## Description

<div><p>You are given an array $a$ of $n$ integers $a_1, a_2, a_3, \ldots, a_n$.</p><p>You have to answer $q$ independent queries, each consisting of two integers $l$ and $r$. </p><ul> <li> Consider the subarray $a[l:r]$ $=$ $[a_l, a_{l+1}, \ldots, a_r]$. You can apply the following operation to the subarray any number of times (possibly zero)- <ol> <li> Choose two integers $L$, $R$ such that $l \le L \le R \le r$ and $R - L + 1$ is <span class="tex-font-style-bf">odd</span>. </li><li> Replace each element in the subarray from $L$ to $R$ with the <span class="tex-font-style-tt">XOR</span> of the elements in the subarray $[L, R]$. </li></ol> </li><li> The answer to the query is the minimum number of operations required to make all elements of the subarray $a[l:r]$ equal to $0$ or $-1$ if it is impossible to make all of them equal to $0$. </li></ul><p>You can find more details about <span class="tex-font-style-tt">XOR</span> operation <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">here</a>.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ $(1 \le n, q \le 2 \cdot 10^5)$ &nbsp;— the length of the array $a$ and the number of queries.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ $(0 \le a_i \lt 2^{30})$ &nbsp;— the elements of the array $a$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i \le r_i \le n)$ &nbsp;— the description of the $i$-th query.</p></div><div class="output-specification"><p>For each query, output a single integer &nbsp;— the answer to that query.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ $(1 \le n, q \le 2 \cdot 10^5)$ &nbsp;— the length of the array $a$ and the number of queries.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ $(0 \le a_i \lt 2^{30})$ &nbsp;— the elements of the array $a$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i \le r_i \le n)$ &nbsp;— the description of the $i$-th query.</p>

## Output

<p>For each query, output a single integer &nbsp;— the answer to that query.</p>





```input1
7 6
3 0 3 3 1 2 3
3 4
4 6
3 7
5 6
1 6
2 2
```




```output1
-1
1
1
-1
2
0
```



## Note

<p>In the <span class="tex-font-style-bf">first query</span>, $l = 3, r = 4$, subarray = $[3, 3]$. We can apply operation only to the subarrays of length $1$, which won't change the array; hence it is impossible to make all elements equal to $0$.</p><p>In the <span class="tex-font-style-bf">second query</span>, $l = 4, r = 6$, subarray = $[3, 1, 2]$. We can choose the whole subarray $(L = 4, R = 6)$ and replace all elements by their XOR $(3 \oplus 1 \oplus 2) = 0$, making the subarray $[0, 0, 0]$.</p><p>In the <span class="tex-font-style-bf">fifth query</span>, $l = 1, r = 6$, subarray = $[3, 0, 3, 3, 1, 2]$. We can make the operations as follows: </p><ol> <li> Choose $L = 4, R = 6$, making the subarray $[3, 0, 3, 0, 0, 0]$. </li><li> Choose $L = 1, R = 5$, making the subarray $[0, 0, 0, 0, 0, 0]$. </li></ol>
