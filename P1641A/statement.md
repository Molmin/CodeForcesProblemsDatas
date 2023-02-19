## Description

<div><p>A sequence of positive integers is called <span class="tex-font-style-it">great</span> for a positive integer $x$, if we can split it into pairs in such a way that in each pair the first number multiplied by $x$ is equal to the second number. More formally, a sequence $a$ of size $n$ is great for a positive integer $x$, if $n$ is even and there exists a permutation $p$ of size $n$, such that for each $i$ ($1 \le i \le \frac{n}{2}$) $a_{p_{2i-1}} \cdot x = a_{p_{2i}}$. </p><p>Sam has a sequence $a$ and a positive integer $x$. Help him to make the sequence great: find the minimum possible number of positive integers that should be added to the sequence $a$ to make it great for the number $x$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 20\,000$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $x$ ($1 \le n \le 2 \cdot 10^5$, $2 \le x \le 10^6$).</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the minimum number of integers that can be added to the end of $a$ to make it a great sequence for the number $x$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 20\,000$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $x$ ($1 \le n \le 2 \cdot 10^5$, $2 \le x \le 10^6$).</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer&nbsp;— the minimum number of integers that can be added to the end of $a$ to make it a great sequence for the number $x$.</p>





```input1
4
4 4
1 16 4 4
6 2
1 2 2 2 4 7
5 3
5 2 3 5 15
9 10
10 10 10 20 1 100 200 2000 3
```




```output1
0
2
3
3
```



## Note

<p>In the first test case, Sam got lucky and the sequence is already great for the number $4$ because you can divide it into such pairs: $(1, 4)$, $(4, 16)$. Thus we can add $0$ numbers.</p><p>In the second test case, you can add numbers $1$ and $14$ to the sequence, then you can divide all $8$ integers into such pairs: $(1, 2)$, $(1, 2)$, $(2, 4)$, $(7, 14)$. It is impossible to add less than $2$ integers to fix the sequence.</p>
