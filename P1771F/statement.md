## Description

<div><p>Hossam gives you a sequence of integers $a_1, \, a_2, \, \dots, \, a_n$ of length $n$. Moreover, he will give you $q$ queries of type $(l, \, r)$. For each query, consider the elements $a_l, \, a_{l + 1}, \, \dots, \, a_r$. Hossam wants to know the <span class="tex-font-style-bf">smallest</span> number in this sequence, such that it occurs in this sequence an <span class="tex-font-style-bf">odd</span> number of times.</p><p>You need to compute the answer for each query before process the next query.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$), the length of the sequence.</p><p>The second line contains $n$ integers $a_1, \, a_2, \, \dots, \, a_n$ ($1 \le a_i \le 10^9$).</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$), the number of queries.</p><p>Each of the next $q$ lines contains two integers $a$ and $b$ ($0 \le a, \, b \le 2 \cdot 10^9$), the numbers used to encode the queries. </p><p>Let $\mathrm{ans}_i$ be the answer on the $i$-th query, and $\mathrm{ans}_0$ be zero. Then $$l_i = a_i \oplus \mathrm{ans}_{i - 1},$$ $$r_i = b_i \oplus \mathrm{ans}_{i - 1},$$ where $l_i, \, r_i$ are parameters of the $i$-th query and $\oplus$ means the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise exclusive or</a> operation. It is guaranteed that $1 \le l \le r \le n$.</p></div><div class="output-specification"><p>For each query, print the smallest number that occurs an odd number of times on the given segment of the sequence.</p><p>If there is no such number, print $0$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$), the length of the sequence.</p><p>The second line contains $n$ integers $a_1, \, a_2, \, \dots, \, a_n$ ($1 \le a_i \le 10^9$).</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$), the number of queries.</p><p>Each of the next $q$ lines contains two integers $a$ and $b$ ($0 \le a, \, b \le 2 \cdot 10^9$), the numbers used to encode the queries. </p><p>Let $\mathrm{ans}_i$ be the answer on the $i$-th query, and $\mathrm{ans}_0$ be zero. Then $$l_i = a_i \oplus \mathrm{ans}_{i - 1},$$ $$r_i = b_i \oplus \mathrm{ans}_{i - 1},$$ where $l_i, \, r_i$ are parameters of the $i$-th query and $\oplus$ means the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise exclusive or</a> operation. It is guaranteed that $1 \le l \le r \le n$.</p>

## Output

<p>For each query, print the smallest number that occurs an odd number of times on the given segment of the sequence.</p><p>If there is no such number, print $0$.</p>





```input1
5
1 2 1 2 2
6
1 2
0 2
0 6
0 5
2 2
3 7
```




```input2
10
51 43 69 48 23 52 48 76 19 55
10
1 1
57 57
54 62
20 27
56 56
79 69
16 21
18 30
25 25
62 61
```




```output1
1
2
1
0
2
2
```




```output2
51
55
19
48
76
19
23
19
55
19
```



## Note

<p>In the example,</p><p>$$l_1 = 1, \, r_1 = 2,$$ $$l_2 = 1, \, r_2 = 3,$$ $$l_3 = 2, \, r_3 = 4,$$ $$l_4 = 1, \, r_4 = 4,$$ $$l_5 = 2, \, r_5 = 2,$$ $$l_6 = 1, \, r_6 = 5.$$</p>
