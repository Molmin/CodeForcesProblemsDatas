## Description

<div><p>Long ago, you thought of two finite <a href="https://en.wikipedia.org/wiki/Arithmetic_progression">arithmetic progressions</a> $A$ and $B$. Then you found out another sequence $C$ containing all elements common to both $A$ and $B$. It is not hard to see that $C$ is also a finite arithmetic progression. After many years, you forgot what $A$ was but remember $B$ and $C$. You are, for some reason, determined to find this lost arithmetic progression. Before you begin this eternal search, you want to know how many different finite arithmetic progressions exist which can be your lost progression $A$. </p><p>Two arithmetic progressions are considered different if they differ in their first term, common difference or number of terms.</p><p>It may be possible that there are infinitely many such progressions, in which case you won't even try to look for them! Print $-1$ in all such cases. </p><p>Even if there are finite number of them, the answer might be very large. So, you are only interested to find the answer modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1\leq t\leq 100$) denoting the number of testcases.</p><p>The first line of each testcase contains three integers $b$, $q$ and $y$ ($-10^9\leq b\leq 10^9$, $1\leq q\leq 10^9$, $2\leq y\leq 10^9$) denoting the first term, common difference and number of terms of $B$ respectively.</p><p>The second line of each testcase contains three integers $c$, $r$ and $z$ ($-10^9\leq c\leq 10^9$, $1\leq r\leq 10^9$, $2\leq z\leq 10^9$) denoting the first term, common difference and number of terms of $C$ respectively.</p></div><div class="output-specification"><p>For each testcase, print a single line containing a single integer.</p><p>If there are infinitely many finite arithmetic progressions which could be your lost progression $A$, print $-1$.</p><p>Otherwise, print the number of finite arithmetic progressions which could be your lost progression $A$ modulo $10^9+7$. In particular, if there are no such finite arithmetic progressions, print $0$.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1\leq t\leq 100$) denoting the number of testcases.</p><p>The first line of each testcase contains three integers $b$, $q$ and $y$ ($-10^9\leq b\leq 10^9$, $1\leq q\leq 10^9$, $2\leq y\leq 10^9$) denoting the first term, common difference and number of terms of $B$ respectively.</p><p>The second line of each testcase contains three integers $c$, $r$ and $z$ ($-10^9\leq c\leq 10^9$, $1\leq r\leq 10^9$, $2\leq z\leq 10^9$) denoting the first term, common difference and number of terms of $C$ respectively.</p>

## Output

<p>For each testcase, print a single line containing a single integer.</p><p>If there are infinitely many finite arithmetic progressions which could be your lost progression $A$, print $-1$.</p><p>Otherwise, print the number of finite arithmetic progressions which could be your lost progression $A$ modulo $10^9+7$. In particular, if there are no such finite arithmetic progressions, print $0$.</p>





```input1
8
-3 1 7
-1 2 4
-9 3 11
0 6 3
2 5 5
7 5 4
2 2 11
10 5 3
0 2 9
2 4 3
-11 4 12
1 12 2
-27 4 7
-17 8 2
-8400 420 1000000000
0 4620 10
```




```output1
0
10
-1
0
-1
21
0
273000
```



## Note

<p>For the first testcase, $B=\{-3,-2,-1,0,1,2,3\}$ and $C=\{-1,1,3,5\}$. There is no such arithmetic progression which can be equal to $A$ because $5$ is not present in $B$ and for any $A$, $5$ should not be present in $C$ also. </p><p>For the second testcase, $B=\{-9,-6,-3,0,3,6,9,12,15,18,21\}$ and $C=\{0,6,12\}$. There are $10$ possible arithmetic progressions which can be $A$: </p><ul> <li> $\{0,6,12\}$ </li><li> $\{0,2,4,6,8,10,12\}$ </li><li> $\{0,2,4,6,8,10,12,14\}$ </li><li> $\{0,2,4,6,8,10,12,14,16\}$ </li><li> $\{-2,0,2,4,6,8,10,12\}$ </li><li> $\{-2,0,2,4,6,8,10,12,14\}$ </li><li> $\{-2,0,2,4,6,8,10,12,14,16\}$ </li><li> $\{-4,-2,0,2,4,6,8,10,12\}$ </li><li> $\{-4,-2,0,2,4,6,8,10,12,14\}$ </li><li> $\{-4,-2,0,2,4,6,8,10,12,14,16\}$ </li></ul><p>For the third testcase, $B=\{2,7,12,17,22\}$ and $C=\{7,12,17,22\}$. There are infinitely many arithmetic progressions which can be $A$ like: </p><ul> <li> $\{7,12,17,22\}$ </li><li> $\{7,12,17,22,27\}$ </li><li> $\{7,12,17,22,27,32\}$ </li><li> $\{7,12,17,22,27,32,37\}$ </li><li> $\{7,12,17,22,27,32,37,42\}$ </li><li> $\ldots$ </li></ul>
