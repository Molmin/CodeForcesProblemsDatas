## Description

<div><p>Neko loves divisors. During the latest number theory lesson, he got an interesting exercise from his math teacher.</p><p>Neko has two integers $a$ and $b$. His goal is to find a non-negative integer $k$ such that the least common multiple of $a+k$ and $b+k$ is the smallest possible. If there are multiple optimal integers $k$, he needs to choose the smallest one.</p><p>Given his mathematical talent, Neko had no trouble getting Wrong Answer on this problem. Can you help him solve it?</p></div><div class="input-specification"><p>The only line contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p></div><div class="output-specification"><p>Print the smallest non-negative integer $k$ ($k \ge 0$) such that the lowest common multiple of $a+k$ and $b+k$ is the smallest possible.</p><p>If there are many possible integers $k$ giving the same value of the least common multiple, print the smallest one.</p></div>

## Input

<p>The only line contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p>

## Output

<p>Print the smallest non-negative integer $k$ ($k \ge 0$) such that the lowest common multiple of $a+k$ and $b+k$ is the smallest possible.</p><p>If there are many possible integers $k$ giving the same value of the least common multiple, print the smallest one.</p>





```input1
6 10
```




```input2
21 31
```




```input3
5 10
```




```output1
2
```




```output2
9
```




```output3
0
```



## Note

<p>In the first test, one should choose $k = 2$, as the least common multiple of $6 + 2$ and $10 + 2$ is $24$, which is the smallest least common multiple possible.</p>
