## Description

<div><p>You are given a string $s$, consisting of lowercase Latin letters.</p><p>You are asked $q$ queries about it: given another string $t$, consisting of lowercase Latin letters, perform the following steps:</p><ol> <li> concatenate $s$ and $t$; </li><li> calculate the prefix function of the resulting string $s+t$; </li><li> print the values of the prefix function on positions $|s|+1, |s|+2, \dots, |s|+|t|$ ($|s|$ and $|t|$ denote the lengths of strings $s$ and $t$, respectively); </li><li> revert the string back to $s$. </li></ol><p>The prefix function of a string $a$ is a sequence $p_1, p_2, \dots, p_{|a|}$, where $p_i$ is the maximum value of $k$ such that $k &lt; i$ and $a[1..k]=a[i-k+1..i]$ ($a[l..r]$ denotes a contiguous substring of a string $a$ from a position $l$ to a position $r$, inclusive). In other words, it's the longest proper prefix of the string $a[1..i]$ that is equal to its suffix of the same length.</p></div><div class="input-specification"><p>The first line contains a non-empty string $s$ ($1 \le |s| \le 10^6$), consisting of lowercase Latin letters.</p><p>The second line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains a query: a non-empty string $t$ ($1 \le |t| \le 10$), consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each query, print the values of the prefix function of a string $s+t$ on positions $|s|+1, |s|+2, \dots, |s|+|t|$.</p></div>

## Input

<p>The first line contains a non-empty string $s$ ($1 \le |s| \le 10^6$), consisting of lowercase Latin letters.</p><p>The second line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains a query: a non-empty string $t$ ($1 \le |t| \le 10$), consisting of lowercase Latin letters.</p>

## Output

<p>For each query, print the values of the prefix function of a string $s+t$ on positions $|s|+1, |s|+2, \dots, |s|+|t|$.</p>





```input1
aba
6
caba
aba
bababa
aaaa
b
forces
```




```input2
aacba
4
aaca
cbbb
aab
ccaca
```




```output1
0 1 2 3 
1 2 3 
2 3 4 5 6 7 
1 1 1 1 
2 
0 0 0 0 0 0
```




```output2
2 2 3 1 
0 0 0 0 
2 2 0 
0 0 1 0 1
```


