## Description

<div><p>Orac is studying number theory, and he is interested in the properties of divisors.</p><p>For two positive integers $a$ and $b$, $a$ is a divisor of $b$ if and only if there exists an integer $c$, such that $a\cdot c=b$.</p><p>For $n \ge 2$, we will denote as $f(n)$ the smallest positive divisor of $n$, except $1$.</p><p>For example, $f(7)=7,f(10)=2,f(35)=5$.</p><p>For the fixed integer $n$, Orac decided to add $f(n)$ to $n$. </p><p>For example, if he had an integer $n=5$, the new value of $n$ will be equal to $10$. And if he had an integer $n=6$, $n$ will be changed to $8$.</p><p>Orac loved it so much, so he decided to repeat this operation several times.</p><p>Now, for two positive integers $n$ and $k$, Orac asked you to add $f(n)$ to $n$ exactly $k$ times (note that $n$ will change after each operation, so $f(n)$ may change too) and tell him the final value of $n$.</p><p>For example, if Orac gives you $n=5$ and $k=2$, at first you should add $f(5)=5$ to $n=5$, so your new value of $n$ will be equal to $n=10$, after that, you should add $f(10)=2$ to $10$, so your new (and the final!) value of $n$ will be equal to $12$.</p><p>Orac may ask you these queries many times.</p></div><div class="input-specification"><p>The first line of the input is a single integer $t\ (1\le t\le 100)$: the number of times that Orac will ask you.</p><p>Each of the next $t$ lines contains two positive integers $n,k\ (2\le n\le 10^6, 1\le k\le 10^9)$, corresponding to a query by Orac.</p><p>It is guaranteed that the total sum of $n$ is at most $10^6$. </p></div><div class="output-specification"><p>Print $t$ lines, the $i$-th of them should contain the final value of $n$ in the $i$-th query by Orac.</p></div>

## Input

<p>The first line of the input is a single integer $t\ (1\le t\le 100)$: the number of times that Orac will ask you.</p><p>Each of the next $t$ lines contains two positive integers $n,k\ (2\le n\le 10^6, 1\le k\le 10^9)$, corresponding to a query by Orac.</p><p>It is guaranteed that the total sum of $n$ is at most $10^6$. </p>

## Output

<p>Print $t$ lines, the $i$-th of them should contain the final value of $n$ in the $i$-th query by Orac.</p>





```input1
3
5 1
8 2
3 4
```




```output1
10
12
12
```



## Note

<p>In the first query, $n=5$ and $k=1$. The divisors of $5$ are $1$ and $5$, the smallest one except $1$ is $5$. Therefore, the only operation adds $f(5)=5$ to $5$, and the result is $10$.</p><p>In the second query, $n=8$ and $k=2$. The divisors of $8$ are $1,2,4,8$, where the smallest one except $1$ is $2$, then after one operation $8$ turns into $8+(f(8)=2)=10$. The divisors of $10$ are $1,2,5,10$, where the smallest one except $1$ is $2$, therefore the answer is $10+(f(10)=2)=12$.</p><p>In the third query, $n$ is changed as follows: $3 \to 6 \to 8 \to 10 \to 12$.</p>
