## Description

<div><p>You are given an array $s$ consisting of $n$ different strings. Each string consists of $m$ lowercase Latin letters.</p><p>You have to respond to $q$ queries. Each query contains a string $t$ of length $m+1$. Count the number of indices $i$, such that the string $t$ can be obtained from the string $s_i$, if it is allowed to insert one letter in an arbitrary position.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5$; $1 \le m \le 10$)&nbsp;— the number of strings in the array and the length of each string.</p><p>The following $n$ lines contain strings $s_i$. All of the given strings are different.</p><p>The next line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>The following $q$ lines contain query strings $t$ of length $m + 1$.</p></div><div class="output-specification"><p>For each query, print the number of indices $i$, such that a string from the query can be obtained from the string $s_i$, if it is allowed to insert one letter in an arbitrary position.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5$; $1 \le m \le 10$)&nbsp;— the number of strings in the array and the length of each string.</p><p>The following $n$ lines contain strings $s_i$. All of the given strings are different.</p><p>The next line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>The following $q$ lines contain query strings $t$ of length $m + 1$.</p>

## Output

<p>For each query, print the number of indices $i$, such that a string from the query can be obtained from the string $s_i$, if it is allowed to insert one letter in an arbitrary position.</p>





```input1
2 1
a
c
4
aa
ca
mm
cf
```




```input2
6 3
dba
abd
cbb
ada
add
bdd
5
ccbb
abdd
adba
bada
dddd
```




```output1
1
2
0
1
```




```output2
1
3
2
1
0
```



## Note

<p>Explanation of the first test of the example:</p><ul> <li> the string <span class="tex-font-style-tt">a</span> can be transformed into <span class="tex-font-style-tt">aa</span> by inserting one letter; </li><li> both strings <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">c</span> can be transformed into <span class="tex-font-style-tt">ca</span> by inserting one letter; </li><li> neither <span class="tex-font-style-tt">a</span> nor <span class="tex-font-style-tt">c</span> can be transformed into <span class="tex-font-style-tt">mm</span> by inserting one letter; </li><li> <span class="tex-font-style-tt">c</span> can be transformed into <span class="tex-font-style-tt">cf</span> by inserting one letter. </li></ul>
