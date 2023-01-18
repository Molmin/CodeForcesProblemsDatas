## Description

<div><p>You are given an array $a$ consisting of $n$ integers $a_1, a_2, \dots, a_n$.</p><p>Your problem is to find such pair of indices $i, j$ ($1 \le i &lt; j \le n$) that $lcm(a_i, a_j)$ is minimum possible.</p><p>$lcm(x, y)$ is the least common multiple of $x$ and $y$ (minimum positive number such that both $x$ and $y$ are divisors of this number).</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 10^6$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^7$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>Print two integers $i$ and $j$ ($1 \le i &lt; j \le n$) such that the value of $lcm(a_i, a_j)$ is minimum among all valid pairs $i, j$. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 10^6$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^7$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>Print two integers $i$ and $j$ ($1 \le i &lt; j \le n$) such that the value of $lcm(a_i, a_j)$ is minimum among all valid pairs $i, j$. If there are multiple answers, you can print any.</p>





```input1
5
2 4 8 3 6
```




```input2
5
5 2 11 3 7
```




```input3
6
2 5 10 1 10 2
```




```output1
1 2
```




```output2
2 4
```




```output3
1 4
```


