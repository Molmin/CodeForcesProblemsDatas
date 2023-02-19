## Description

<div><p>Gregor is learning about RSA cryptography, and although he doesn't understand how RSA works, he is now fascinated with prime numbers and factoring them.</p><p>Gregor's favorite <span class="tex-font-style-bf">prime</span> number is $P$. Gregor wants to find two <span class="tex-font-style-it">bases</span> of $P$. Formally, Gregor is looking for two integers $a$ and $b$ which satisfy both of the following properties.</p><ul> <li> $P \bmod a = P \bmod b$, where $x \bmod y$ denotes the remainder when $x$ is divided by $y$, and </li><li> $2 \le a &lt; b \le P$. </li></ul><p>Help Gregor find two bases of his favorite prime number!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$).</p><p>Each subsequent line contains the integer $P$ ($5 \le P \le {10}^9$), with $P$ guaranteed to be prime.</p></div><div class="output-specification"><p>Your output should consist of $t$ lines. Each line should consist of two integers $a$ and $b$ ($2 \le a &lt; b \le P$). If there are multiple possible solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$).</p><p>Each subsequent line contains the integer $P$ ($5 \le P \le {10}^9$), with $P$ guaranteed to be prime.</p>

## Output

<p>Your output should consist of $t$ lines. Each line should consist of two integers $a$ and $b$ ($2 \le a &lt; b \le P$). If there are multiple possible solutions, print any.</p>





```input1
2
17
5
```




```output1
3 5
2 4
```



## Note

<p>The first query is $P=17$. $a=3$ and $b=5$ are valid <span class="tex-font-style-it">bases</span> in this case, because $17 \bmod 3 = 17 \bmod 5 = 2$. There are other pairs which work as well.</p><p>In the second query, with $P=5$, the only solution is $a=2$ and $b=4$.</p>
