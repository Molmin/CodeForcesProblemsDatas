## Description

<div><p>Once upon a time, Oolimry saw a suffix array. He wondered how many strings can produce this suffix array. </p><p>More formally, given a suffix array of length $n$ and having an alphabet size $k$, count the number of strings that produce such a suffix array. </p><p>Let $s$ be a string of length $n$. Then the $i$-th suffix of $s$ is the substring $s[i \ldots n-1]$. A suffix array is the array of integers that represent the starting indexes of all the suffixes of a given string, after the suffixes are sorted in the lexicographic order. For example, the suffix array of <span class="tex-font-style-tt">oolimry</span> is $[3,2,4,1,0,5,6]$ as the array of sorted suffixes is $[\texttt{imry},\texttt{limry},\texttt{mry},\texttt{olimry},\texttt{oolimry},\texttt{ry},\texttt{y}]$. </p><p>A string $x$ is lexicographically smaller than string $y$, if either $x$ is a prefix of $y$ (and $x\neq y$), or there exists such $i$ that $x_i &lt; y_i$, and for any $1\leq j &lt; i$ , $x_j = y_j$.</p></div><div class="input-specification"><p>The first line contain 2 integers $n$ and $k$ ($1 \leq n \leq 200000,1 \leq k \leq 200000$) — the length of the suffix array and the alphabet size respectively.</p><p>The second line contains $n$ integers $s_0, s_1, s_2, \ldots, s_{n-1}$ ($0 \leq s_i \leq n-1$) <span class="tex-font-style-bf">where $s_i$ is the $i$-th element of the suffix array</span> i.e. the starting position of the $i$-th lexicographically smallest suffix. It is guaranteed that for all $0 \leq i&lt; j \leq n-1$, $s_i \neq s_j$.</p></div><div class="output-specification"><p>Print how many strings produce such a suffix array. Since the number can be very large, print the answer modulo $998244353$.</p></div>

## Input

<p>The first line contain 2 integers $n$ and $k$ ($1 \leq n \leq 200000,1 \leq k \leq 200000$) — the length of the suffix array and the alphabet size respectively.</p><p>The second line contains $n$ integers $s_0, s_1, s_2, \ldots, s_{n-1}$ ($0 \leq s_i \leq n-1$) <span class="tex-font-style-bf">where $s_i$ is the $i$-th element of the suffix array</span> i.e. the starting position of the $i$-th lexicographically smallest suffix. It is guaranteed that for all $0 \leq i&lt; j \leq n-1$, $s_i \neq s_j$.</p>

## Output

<p>Print how many strings produce such a suffix array. Since the number can be very large, print the answer modulo $998244353$.</p>





```input1
3 2
0 2 1
```




```input2
5 1
0 1 2 3 4
```




```input3
6 200000
0 1 2 3 4 5
```




```input4
7 6
3 2 4 1 0 5 6
```




```output1
1
```




```output2
0
```




```output3
822243495
```




```output4
36
```



## Note

<p>In the first test case, "abb" is the only possible solution. </p><p>In the second test case, it can be easily shown no possible strings exist as all the letters have to be equal. </p><p>In the fourth test case, one possible string is "ddbacef".</p><p>Please remember to print your answers modulo $998244353$.</p>
