## Description

<div><p>Baby Ehab has a piece of Cut and Stick with an array $a$ of length $n$ written on it. He plans to grab a pair of scissors and do the following to it:</p><ul> <li> pick a range $(l, r)$ and cut out every element $a_l$, $a_{l + 1}$, ..., $a_r$ in this range; </li><li> stick some of the elements together in the same order they were in the array; </li><li> end up with multiple pieces, where every piece contains some of the elements and every element belongs to some piece. </li></ul><p>More formally, he partitions the sequence $a_l$, $a_{l + 1}$, ..., $a_r$ into subsequences. He thinks a partitioning is beautiful if for every piece (subsequence) it holds that, if it has length $x$, then no value occurs strictly more than $\lceil \frac{x}{2} \rceil$ times in it.</p><p>He didn't pick a range yet, so he's wondering: for $q$ ranges $(l, r)$, what is the minimum number of pieces he needs to partition the elements $a_l$, $a_{l + 1}$, ..., $a_r$ into so that the partitioning is beautiful.</p><p>A sequence $b$ is a subsequence of an array $a$ if $b$ can be obtained from $a$ by deleting some (possibly zero) elements. Note that it does <span class="tex-font-style-bf">not</span> have to be contiguous.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n,q \le 3 \cdot 10^5$)&nbsp;— the length of the array $a$ and the number of queries.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_{n}$ ($1 \le a_i \le n$)&nbsp;— the elements of the array $a$.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le n$)&nbsp;— the range of this query.</p></div><div class="output-specification"><p>For each query, print the minimum number of subsequences you need to partition this range into so that the partitioning is beautiful. We can prove such partitioning always exists.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n,q \le 3 \cdot 10^5$)&nbsp;— the length of the array $a$ and the number of queries.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_{n}$ ($1 \le a_i \le n$)&nbsp;— the elements of the array $a$.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le n$)&nbsp;— the range of this query.</p>

## Output

<p>For each query, print the minimum number of subsequences you need to partition this range into so that the partitioning is beautiful. We can prove such partitioning always exists.</p>





```input1
6 2
1 3 2 3 3 2
1 6
2 5
```




```output1
1
2
```



## Note

<p>In the first query, you can just put the whole array in one subsequence, since its length is $6$, and no value occurs more than $3$ times in it.</p><p>In the second query, the elements of the query range are $[3,2,3,3]$. You can't put them all in one subsequence, since its length is $4$, and $3$ occurs more than $2$ times. However, you can partition it into two subsequences: $[3]$ and $[2,3,3]$.</p>
