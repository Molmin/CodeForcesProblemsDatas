## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>You are given two integers $c$ and $n$. The jury has a <span class="tex-font-style-bf">randomly generated</span> set $A$ of distinct positive integers not greater than $c$ (it is generated from all such possible sets with equal probability). The size of $A$ is equal to $n$.</p><p>Your task is to guess the set $A$. In order to guess it, you can ask at most $\lceil 0.65 \cdot c \rceil$ queries.</p><p>In each query, you choose a single integer $1 \le x \le c$. As the answer to this query you will be given the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise xor sum</a> of all $y$, such that $y \in A$ and $gcd(x, y) = 1$ (i.e. $x$ and $y$ are coprime). If there is no such $y$ this xor sum is equal to $0$.</p><p>You can ask all queries at the beginning and you will receive the answers to all your queries. After that, you won't have the possibility to ask queries.</p><p>You should find any set $A'$, such that $|A'| = n$ and $A'$ and $A$ have the same answers for all $c$ possible queries.</p></div><div class="input-specification"><p>Firstly you are given two integers $c$ and $n$ ($100 \le c \le 10^6$, $0 \le n \le c$).</p></div><div><h2>Interaction</h2><p>In the first line you should print an integer $q$ $(0 \le q \le \lceil 0.65 \cdot c \rceil)$&nbsp;— the number of queries you want to ask. After that in the same line print $q$ integers $x_1, x_2, \ldots, x_q$ $(1 \le x_i \le c)$&nbsp;— the queries.</p><p>For these queries you should read $q$ integers, $i$-th of them is the answer to the described query for $x = x_i$.</p><p>After that you should print $n$ distinct integers $A'_1, A'_2, \ldots, A'_n$&nbsp;— the set $A'$ you found.</p><p>If there are different sets $A'$ that have the same answers for all possible queries, print any of them.</p><p>If you will ask more than $\lceil 0.65 \cdot c \rceil$ queries or if the queries will be invalid, the interactor will terminate immediately and your program will receive verdict <span class="tex-font-style-tt">Wrong Answer</span>.</p><p>After printing the queries and answers do not forget to output end of line and flush the output buffer. Otherwise, you will get the <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict. To do flush use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> Read documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>You cannot make hacks in this problem.</p></div>

## Input

<p>Firstly you are given two integers $c$ and $n$ ($100 \le c \le 10^6$, $0 \le n \le c$).</p>





```input1
10 6

1 4 2 11 4 4 4
```




```output1
7 10 2 3 5 7 1 6

1 4 5 6 8 10
```



## Note

<p>The sample is made only for you to understand the interaction protocol. <span class="tex-font-style-bf">Your solution will not be tested on the sample.</span></p><p>In the sample $A = \{1, 4, 5, 6, 8, 10\}$. $7$ queries are made, $7 \le \lceil 0.65 \cdot 10 \rceil = 7$, so the query limit is not exceeded.</p><p>Answers for the queries: </p><ul> <li> For $10$: $1$ is the only number in the set $A$ coprime with $10$, so the answer is $1$ </li><li> For $2$: $1_{10} \oplus 5_{10} = 001_2 \oplus 101_2 = 4_{10}$, where $\oplus$ is the bitwise xor </li><li> For $3$: $1_{10} \oplus 4_{10} \oplus 5_{10} \oplus 8_{10} \oplus 10_{10} = 0001_2 \oplus 0100_2 \oplus 0101_2 \oplus 1000_2 \oplus 1010_2 = 2_{10}$ </li><li> For $5$: $1_{10} \oplus 4_{10} \oplus 6_{10} \oplus 8_{10} = 0001_2 \oplus 0100_2 \oplus 0110_2 \oplus 1000_2 = 11_{10}$ </li><li> For $7$: $1_{10} \oplus 4_{10} \oplus 5_{10} \oplus 6_{10} \oplus 8_{10} \oplus 10_{10} = 0001_2 \oplus 0100_2 \oplus 0101_2 \oplus 0110_2 \oplus 1000_2 \oplus 1010_2 = 4_{10}$ </li><li> For $1$: $1_{10} \oplus 4_{10} \oplus 5_{10} \oplus 6_{10} \oplus 8_{10} \oplus 10_{10} = 0001_2 \oplus 0100_2 \oplus 0101_2 \oplus 0110_2 \oplus 1000_2 \oplus 1010_2 = 4_{10}$ </li><li> For $6$: $1_{10} \oplus 5_{10} = 0001_2 \oplus 0101_2 = 4_{10}$ </li></ul>
