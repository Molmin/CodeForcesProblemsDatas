## Description

<div><p>A sequence of $n$ non-negative integers ($n \ge 2$) $a_1, a_2, \dots, a_n$ is called good if for all $i$ from $1$ to $n-1$ the following condition holds true: $$a_1 \: \&amp; \: a_2 \: \&amp; \: \dots \: \&amp; \: a_i = a_{i+1} \: \&amp; \: a_{i+2} \: \&amp; \: \dots \: \&amp; \: a_n,$$ where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>You are given an array $a$ of size $n$ ($n \geq 2$). Find the number of permutations $p$ of numbers ranging from $1$ to $n$, for which the sequence $a_{p_1}$, $a_{p_2}$, ... ,$a_{p_n}$ is good. Since this number can be large, output it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$), denoting the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) — the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $t$ lines, where the $i$-th line contains the number of good permutations in the $i$-th test case modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$), denoting the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) — the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $t$ lines, where the $i$-th line contains the number of good permutations in the $i$-th test case modulo $10^9 + 7$.</p>





```input1
4
3
1 1 1
5
1 2 3 4 5
5
0 2 0 3 0
4
1 3 5 1
```




```output1
6
0
36
4
```



## Note

<p>In the first test case, since all the numbers are equal, whatever permutation we take, the sequence is good. There are a total of $6$ permutations possible with numbers from $1$ to $3$: $[1,2,3]$, $[1,3,2]$, $[2,1,3]$, $[2,3,1]$, $[3,1,2]$, $[3,2,1]$.</p><p>In the second test case, it can be proved that no permutation exists for which the sequence is good.</p><p>In the third test case, there are a total of $36$ permutations for which the sequence is good. One of them is the permutation $[1,5,4,2,3]$ which results in the sequence $s=[0,0,3,2,0]$. This is a good sequence because </p><ul> <li> $ s_1 = s_2 \: \&amp; \: s_3 \: \&amp; \: s_4 \: \&amp; \: s_5 = 0$, </li><li> $ s_1 \: \&amp; \: s_2 = s_3 \: \&amp; \: s_4 \: \&amp; \: s_5 = 0$, </li><li> $ s_1 \: \&amp; \: s_2 \: \&amp; \: s_3 = s_4 \: \&amp; \: s_5 = 0$, </li><li> $ s_1 \: \&amp; \: s_2 \: \&amp; \: s_3 \: \&amp; \: s_4 = s_5 = 0$. </li></ul><p> </p>
