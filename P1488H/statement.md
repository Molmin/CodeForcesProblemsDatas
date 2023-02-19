## Description

<div><p>You are given an integer $n$ and a sequence $a$ of $n-1$ integers, each element is either $0$ or $1$.</p><p>You are asked to build a string of length $n$ such that: </p><ul> <li> each letter is one of "<span class="tex-font-style-tt">abcd</span>"; </li><li> if $a_i=1$, then the $i$-th suffix of the string is lexicographically smaller than the $(i+1)$-th suffix; </li><li> if $a_i=0$, then the $i$-th suffix of the string is lexicographically greater than the $(i+1)$-th suffix. </li></ul><p>You will be asked $q$ queries of form: </p><ul> <li> $i$ ($1 \le i \le n - 1$)&nbsp;— flip the value of $a_i$ (if $a_i=0$, then set $a_i$ to $1$, and vice versa). </li></ul><p>After each query print the number of different strings that satisfy the given constraints modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 10^5$; $1 \le q \le 10^5$)&nbsp;— the length of the string and the number of queries.</p><p>The second line contains $n-1$ integers $a_1, a_2, \dots, a_{n-1}$ ($a_i \in \{0, 1\}$)&nbsp;— the constraints on suffixes of the string.</p><p>Each of the next $q$ lines contains a query: an integer $i$ ($1 \le i \le n - 1$)&nbsp;— flip the value of $a_i$ (if $a_i=0$, then set $a_i$ to $1$, and vice versa).</p></div><div class="output-specification"><p>After each query print the number of different strings that satisfy the given constraints modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 10^5$; $1 \le q \le 10^5$)&nbsp;— the length of the string and the number of queries.</p><p>The second line contains $n-1$ integers $a_1, a_2, \dots, a_{n-1}$ ($a_i \in \{0, 1\}$)&nbsp;— the constraints on suffixes of the string.</p><p>Each of the next $q$ lines contains a query: an integer $i$ ($1 \le i \le n - 1$)&nbsp;— flip the value of $a_i$ (if $a_i=0$, then set $a_i$ to $1$, and vice versa).</p>

## Output

<p>After each query print the number of different strings that satisfy the given constraints modulo $998\,244\,353$.</p>





```input1
2 2
0
1
1
```




```input2
3 4
0 0
1
2
1
2
```




```input3
10 10
0 0 0 1 1 1 0 1 0
4
1
8
4
2
9
5
6
6
8
```




```output1
6
10
```




```output2
20
10
14
20
```




```output3
1815
3201
2710
2776
2290
1644
2668
1271
2668
2436
```



## Note

<p>The $i$-th suffix of a string is a continuous substring that starts from the $i$-th position and ends in the last position.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul><p>Two strings $a$ and $b$ of length $n$ differ if there exists a position $i$ such that $a_i \neq b_i$.</p>
