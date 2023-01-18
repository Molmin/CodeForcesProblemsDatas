## Description

<div><p>You are given an array which is initially empty. You need to perform $n$ operations of the given format: </p><ul> <li> "$a$ $l$ $r$ $k$": append $a$ to the end of the array. After that count the number of integer pairs $x, y$ such that $l \leq x \leq y \leq r$ and $\operatorname{mex}(a_{x}, a_{x+1}, \ldots, a_{y}) = k$. </li></ul><p>The elements of the array are numerated from $1$ in the order they are added to the array.</p><p>To make this problem more tricky we don't say your real parameters of the queries. Instead your are given $a'$, $l'$, $r'$, $k'$. To get $a$, $l$, $r$, $k$ on the $i$-th operation you need to perform the following: </p><ul> <li> $a := (a' + lans) \bmod(n + 1)$, </li><li> $l := (l' + lans) \bmod{i} + 1$, </li><li> $r := (r' + lans) \bmod{i} + 1$, </li><li> if $l &gt; r$ swap $l$ and $r$, </li><li> $k := (k' + lans) \bmod(n + 1)$, </li></ul> where $lans$ is the answer to the previous operation, initially $lans$ is equal to zero. $i$ is the id of the operation, operations are numbered from $1$.<p>The $\operatorname{mex}(S)$, where $S$ is a multiset of non-negative integers, is the smallest non-negative integer which does not appear in the set. For example, $\operatorname{mex}(\{2, 2, 3\}) = 0$ and $\operatorname{mex} (\{0, 1, 4, 1, 6\}) = 2$. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The next $n$ lines contain the description of queries.</p><p>Each of them $n$ lines contains four non-negative integers $a'$, $l'$, $r'$, $k'$ ($0, \leq a', l', r', k' \leq 10^9$), describing one operation.</p></div><div class="output-specification"><p>For each query print a single integer&nbsp;— the answer to this query.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The next $n$ lines contain the description of queries.</p><p>Each of them $n$ lines contains four non-negative integers $a'$, $l'$, $r'$, $k'$ ($0, \leq a', l', r', k' \leq 10^9$), describing one operation.</p>

## Output

<p>For each query print a single integer&nbsp;— the answer to this query.</p>





```input1
5
0 0 0 1
0 1 0 5
5 2 1 0
5 2 1 0
2 4 3 3
```




```input2
5
2 0 0 2
2 0 1 1
0 0 2 0
3 2 2 0
0 2 3 0
```




```output1
1
1
2
6
3
```




```output2
0
0
3
0
0
```



## Note

<p>For the first example the decoded values of $a$, $l$, $r$, $k$ are the following:</p><p>$a_1=0,l_1=1,r_1=1,k_1=1$</p><p>$a_2=1,l_2=1,r_2=2,k_2=0$</p><p>$a_3=0,l_3=1,r_3=3,k_3=1$</p><p>$a_4=1,l_4=1,r_4=4,k_4=2$</p><p>$a_5=2,l_5=1,r_5=5,k_5=3$</p><p>For the second example the decoded values of $a$, $l$, $r$, $k$ are the following:</p><p>$a_1=2,l_1=1,r_1=1,k_1=2$</p><p>$a_2=2,l_2=1,r_2=2,k_2=1$</p><p>$a_3=0,l_3=1,r_3=3,k_3=0$</p><p>$a_4=0,l_4=2,r_4=2,k_4=3$</p><p>$a_5=0,l_5=3,r_5=4,k_5=0$</p>
