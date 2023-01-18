## Description

<div><p>Given a positive integer $m$, we say that a sequence $x_1, x_2, \dots, x_n$ of positive integers is $m$-cute if for every index $i$ such that $2 \le i \le n$ it holds that $x_i = x_{i - 1} + x_{i - 2} + \dots + x_1 + r_i$ for some positive integer $r_i$ satisfying $1 \le r_i \le m$.</p><p>You will be given $q$ queries consisting of three positive integers $a$, $b$ and $m$. For each query you must determine whether or not there exists an $m$-cute sequence whose first term is $a$ and whose last term is $b$. If such a sequence exists, you must additionally find an example of it.</p></div><div class="input-specification"><p>The first line contains an integer number $q$ ($1 \le q \le 10^3$)&nbsp;— the number of queries.</p><p>Each of the following $q$ lines contains three integers $a$, $b$, and $m$ ($1 \le a, b, m \le 10^{14}$, $a \leq b$), describing a single query.</p></div><div class="output-specification"><p>For each query, if no $m$-cute sequence whose first term is $a$ and whose last term is $b$ exists, print $-1$.</p><p>Otherwise print an integer $k$ ($1 \le k \leq 50$), followed by $k$ integers $x_1, x_2, \dots, x_k$ ($1 \le x_i \le 10^{14}$). These integers must satisfy $x_1 = a$, $x_k = b$, and that the sequence $x_1, x_2, \dots, x_k$ is $m$-cute.</p><p>It can be shown that under the problem constraints, for each query either no $m$-cute sequence exists, or there exists one with at most $50$ terms.</p><p>If there are multiple possible sequences, you may print any of them.</p></div>

## Input

<p>The first line contains an integer number $q$ ($1 \le q \le 10^3$)&nbsp;— the number of queries.</p><p>Each of the following $q$ lines contains three integers $a$, $b$, and $m$ ($1 \le a, b, m \le 10^{14}$, $a \leq b$), describing a single query.</p>

## Output

<p>For each query, if no $m$-cute sequence whose first term is $a$ and whose last term is $b$ exists, print $-1$.</p><p>Otherwise print an integer $k$ ($1 \le k \leq 50$), followed by $k$ integers $x_1, x_2, \dots, x_k$ ($1 \le x_i \le 10^{14}$). These integers must satisfy $x_1 = a$, $x_k = b$, and that the sequence $x_1, x_2, \dots, x_k$ is $m$-cute.</p><p>It can be shown that under the problem constraints, for each query either no $m$-cute sequence exists, or there exists one with at most $50$ terms.</p><p>If there are multiple possible sequences, you may print any of them.</p>





```input1
2
5 26 2
3 9 1
```




```output1
4 5 6 13 26
-1
```



## Note

<p>Consider the sample. In the first query, the sequence $5, 6, 13, 26$ is valid since $6 = 5 + \bf{\color{blue} 1}$, $13 = 6 + 5 + {\bf\color{blue} 2}$ and $26 = 13 + 6 + 5 + {\bf\color{blue} 2}$ have the bold values all between $1$ and $2$, so the sequence is $2$-cute. Other valid sequences, such as $5, 7, 13, 26$ are also accepted.</p><p>In the second query, the only possible $1$-cute sequence starting at $3$ is $3, 4, 8, 16, \dots$, which does not contain $9$.</p>
