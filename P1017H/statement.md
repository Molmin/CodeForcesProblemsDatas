## Description

<div><p>In "<span class="tex-font-style-tt">The Man in the High Castle</span>" world, there are $m$ different film endings. </p><p>Abendsen owns a storage and a shelf. At first, he has $n$ ordered films on the shelf. In the $i$-th month he will do:</p><ol><li> Empty the storage.</li><li> Put $k_i \cdot m$ films into the storage, $k_i$ films for each ending.</li><li> He will think about a question: if he puts all the films from the shelf into the storage, then randomly picks $n$ films (from all the films in the storage) and rearranges them on the shelf, what is the probability that sequence of endings in $[l_i, r_i]$ on the shelf will not be changed? Notice, he just thinks about this question, so the shelf will not actually be changed.</li></ol><p>Answer all Abendsen's questions.</p><p>Let the probability be fraction $P_i$. Let's say that the total number of ways to take $n$ films from the storage for $i$-th month is $A_i$, so $P_i \cdot A_i$ is always an integer. Print for each month $P_i \cdot A_i \pmod {998244353}$.</p><p>$998244353$ is a prime number and it is equal to $119 \cdot 2^{23} + 1$.</p><p>It is guaranteed that there will be only no more than $100$ different $k$ values.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $q$ ($1 \le n, m, q \le 10^5$, $n+q\leq 10^5$)&nbsp;— the number of films on the shelf initially, the number of endings, and the number of months.</p><p>The second line contains $n$ integers $e_1, e_2, \ldots, e_n$ ($1\leq e_i\leq m$)&nbsp;— the ending of the $i$-th film on the shelf.</p><p>Each of the next $q$ lines contains three integers $l_i$, $r_i$, and $k_i$ ($1 \le l_i \le r_i \le n, 0 \le k_i \le 10^5$)&nbsp;— the $i$-th query.</p><p>It is guaranteed that there will be only no more than $100$ different $k$ values.</p></div><div class="output-specification"><p>Print the answer for each question in a separate line.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $q$ ($1 \le n, m, q \le 10^5$, $n+q\leq 10^5$)&nbsp;— the number of films on the shelf initially, the number of endings, and the number of months.</p><p>The second line contains $n$ integers $e_1, e_2, \ldots, e_n$ ($1\leq e_i\leq m$)&nbsp;— the ending of the $i$-th film on the shelf.</p><p>Each of the next $q$ lines contains three integers $l_i$, $r_i$, and $k_i$ ($1 \le l_i \le r_i \le n, 0 \le k_i \le 10^5$)&nbsp;— the $i$-th query.</p><p>It is guaranteed that there will be only no more than $100$ different $k$ values.</p>

## Output

<p>Print the answer for each question in a separate line.</p>





```input1
6 4 4
1 2 3 4 4 4
1 4 0
1 3 2
1 4 2
1 5 2

```




```input2
5 5 3
1 2 3 4 5
1 2 100000
1 4 4
3 5 5

```




```output1
6
26730
12150
4860

```




```output2
494942218
13125
151632

```



## Note

<p>In the first sample in the second query, after adding $2 \cdot m$ films into the storage, the storage will look like this: $\{1, 1, 1, 2, 2, 2, 3, 3, 3, 4, 4, 4, 4, 4\}$.</p><p>There are $26730$ total ways of choosing the films so that $e_l, e_{l+1}, \ldots, e_r$ will not be changed, for example, $[1, 2, 3, 2, 2]$ and $[1, 2, 3, 4, 3]$ are such ways.</p><p>There are $2162160$ total ways of choosing the films, so you're asked to print $(\frac{26730}{2162160} \cdot 2162160) \mod 998244353 = 26730$.</p>
