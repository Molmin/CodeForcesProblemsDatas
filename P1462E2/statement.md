## Description

<div><p><span class="tex-font-style-bf">This is the hard version of this problem. The only difference between the easy and hard versions is the constraints on $k$ and $m$. In this version of the problem, you need to output the answer by modulo $10^9+7$.</span></p><p>You are given a sequence $a$ of length $n$ consisting of integers from $1$ to $n$. <span class="tex-font-style-bf">The sequence may contain duplicates (i.e. some elements can be equal)</span>.</p><p>Find the number of tuples of $m$ elements such that the maximum number in the tuple differs from the minimum by no more than $k$. Formally, you need to find the number of tuples of $m$ indices $i_1 &lt; i_2 &lt; \ldots &lt; i_m$, such that</p><p>$$\max(a_{i_1}, a_{i_2}, \ldots, a_{i_m}) - \min(a_{i_1}, a_{i_2}, \ldots, a_{i_m}) \le k.$$</p><p>For example, if $n=4$, $m=3$, $k=2$, $a=[1,2,4,3]$, then there are two such triples ($i=1, j=2, z=4$ and $i=2, j=3, z=4$). If $n=4$, $m=2$, $k=1$, $a=[1,1,1,1]$, then all six possible pairs are suitable.</p><p><span class="tex-font-style-bf">As the result can be very large, you should print the value modulo $10^9 + 7$ (the remainder when divided by $10^9 + 7$)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains three integers $n$, $m$, $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le m \le 100$, $1 \le k \le n$)&nbsp;— the length of the sequence $a$, number of elements in the tuples and the maximum difference of elements in the tuple.</p><p>The next line contains $n$ integers $a_1, a_2,\ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the sequence $a$.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $t$ answers to the given test cases. Each answer is the required number of tuples of $m$ elements modulo $10^9 + 7$, such that the maximum value in the tuple differs from the minimum by no more than $k$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains three integers $n$, $m$, $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le m \le 100$, $1 \le k \le n$)&nbsp;— the length of the sequence $a$, number of elements in the tuples and the maximum difference of elements in the tuple.</p><p>The next line contains $n$ integers $a_1, a_2,\ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the sequence $a$.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $t$ answers to the given test cases. Each answer is the required number of tuples of $m$ elements modulo $10^9 + 7$, such that the maximum value in the tuple differs from the minimum by no more than $k$.</p>





```input1
4
4 3 2
1 2 4 3
4 2 1
1 1 1 1
1 1 1
1
10 4 3
5 6 1 3 2 9 8 1 2 4
```




```output1
2
6
1
20
```


