## Description

<div><p>Recently Lynyrd and Skynyrd went to a shop where Lynyrd bought a permutation $p$ of length $n$, and Skynyrd bought an array $a$ of length $m$, consisting of integers from $1$ to $n$. </p><p>Lynyrd and Skynyrd became bored, so they asked you $q$ queries, each of which has the following form: "does the subsegment of $a$ from the $l$-th to the $r$-th positions, inclusive, have a subsequence that is a cyclic shift of $p$?" Please answer the queries.</p><p>A <span class="tex-font-style-it">permutation</span> of length $n$ is a sequence of $n$ integers such that each integer from $1$ to $n$ appears exactly once in it.</p><p>A <span class="tex-font-style-it">cyclic shift</span> of a permutation $(p_1, p_2, \ldots, p_n)$ is a permutation $(p_i, p_{i + 1}, \ldots, p_{n}, p_1, p_2, \ldots, p_{i - 1})$ for some $i$ from $1$ to $n$. For example, a permutation $(2, 1, 3)$ has three distinct cyclic shifts: $(2, 1, 3)$, $(1, 3, 2)$, $(3, 2, 1)$.</p><p>A <span class="tex-font-style-it">subsequence</span> of a subsegment of array $a$ from the $l$-th to the $r$-th positions, inclusive, is a sequence $a_{i_1}, a_{i_2}, \ldots, a_{i_k}$ for some $i_1, i_2, \ldots, i_k$ such that $l \leq i_1 &lt; i_2 &lt; \ldots &lt; i_k \leq r$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, $q$ ($1 \le n, m, q \le 2 \cdot 10^5$)&nbsp;— the length of the permutation $p$, the length of the array $a$ and the number of queries.</p><p>The next line contains $n$ integers from $1$ to $n$, where the $i$-th of them is the $i$-th element of the permutation. Each integer from $1$ to $n$ appears exactly once.</p><p>The next line contains $m$ integers from $1$ to $n$, the $i$-th of them is the $i$-th element of the array $a$.</p><p>The next $q$ lines describe queries. The $i$-th of these lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le m$), meaning that the $i$-th query is about the subsegment of the array from the $l_i$-th to the $r_i$-th positions, inclusive.</p></div><div class="output-specification"><p>Print a single string of length $q$, consisting of $0$ and $1$, the digit on the $i$-th positions should be $1$, if the subsegment of array $a$ from the $l_i$-th to the $r_i$-th positions, inclusive, contains a subsequence that is a cyclic shift of $p$, and $0$ otherwise.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, $q$ ($1 \le n, m, q \le 2 \cdot 10^5$)&nbsp;— the length of the permutation $p$, the length of the array $a$ and the number of queries.</p><p>The next line contains $n$ integers from $1$ to $n$, where the $i$-th of them is the $i$-th element of the permutation. Each integer from $1$ to $n$ appears exactly once.</p><p>The next line contains $m$ integers from $1$ to $n$, the $i$-th of them is the $i$-th element of the array $a$.</p><p>The next $q$ lines describe queries. The $i$-th of these lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le m$), meaning that the $i$-th query is about the subsegment of the array from the $l_i$-th to the $r_i$-th positions, inclusive.</p>

## Output

<p>Print a single string of length $q$, consisting of $0$ and $1$, the digit on the $i$-th positions should be $1$, if the subsegment of array $a$ from the $l_i$-th to the $r_i$-th positions, inclusive, contains a subsequence that is a cyclic shift of $p$, and $0$ otherwise.</p>





```input1
3 6 3
2 1 3
1 2 3 1 2 3
1 5
2 6
3 5

```




```input2
2 4 3
2 1
1 1 2 2
1 2
2 3
3 4

```




```output1
110

```




```output2
010

```



## Note

<p>In the first example the segment from the $1$-st to the $5$-th positions is $1, 2, 3, 1, 2$. There is a subsequence $1, 3, 2$ that is a cyclic shift of the permutation. The subsegment from the $2$-nd to the $6$-th positions also contains a subsequence $2, 1, 3$ that is equal to the permutation. The subsegment from the $3$-rd to the $5$-th positions is $3, 1, 2$, there is only one subsequence of length $3$ ($3, 1, 2$), but it is not a cyclic shift of the permutation.</p><p>In the second example the possible cyclic shifts are $1, 2$ and $2, 1$. The subsegment from the $1$-st to the $2$-nd positions is $1, 1$, its subsequences are not cyclic shifts of the permutation. The subsegment from the $2$-nd to the $3$-rd positions is $1, 2$, it coincides with the permutation. The subsegment from the $3$ to the $4$ positions is $2, 2$, its subsequences are not cyclic shifts of the permutation.</p>
