## Description

<div><p>You are given two arrays of integers $a_1, a_2, \ldots, a_n$ and $b_1, b_2, \ldots, b_n$. You need to handle $q$ queries of the following two types:</p><ul><li> $1$ $l$ $r$ $x$: assign $a_i := x$ for all $l \leq i \leq r$;</li><li> $2$ $l$ $r$: find the minimum value of the following expression among all $l \leq i \leq r$: $$\frac{\operatorname{lcm}(a_i, b_i)}{\gcd(a_i, b_i)}.$$</li></ul><p>In this problem $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of $x$ and $y$, and $\operatorname{lcm}(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple</a> of $x$ and $y$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \leq n, q \leq 5 \cdot 10^4$) — the number of numbers in the arrays $a$ and $b$ and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 5 \cdot 10^4$) — the elements of the array $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 5 \cdot 10^4$) — the elements of the array $b$.</p><p>Then $q$ lines follow, $j$-th of which starts with an integer $t_j$ ($1 \leq t_j \leq 2$) and means that the $j$-th query has type $t_j$.</p><p>If $t_j = 1$, it is followed by three integers $l_j$, $r_j$, and $x_j$ ($1 \leq l_j \leq r_j \leq n$, $1 \leq x_j \leq 5 \cdot 10^4$).</p><p>If $t_j = 2$, it is followed by two integers $l_j$ and $r_j$ ($1 \leq l_j \leq r_j \leq n$).</p><p>It is guaranteed that there is at least one query of type $2$.</p></div><div class="output-specification"><p>For each query of the second type, output the minimum value of the expression.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \leq n, q \leq 5 \cdot 10^4$) — the number of numbers in the arrays $a$ and $b$ and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 5 \cdot 10^4$) — the elements of the array $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 5 \cdot 10^4$) — the elements of the array $b$.</p><p>Then $q$ lines follow, $j$-th of which starts with an integer $t_j$ ($1 \leq t_j \leq 2$) and means that the $j$-th query has type $t_j$.</p><p>If $t_j = 1$, it is followed by three integers $l_j$, $r_j$, and $x_j$ ($1 \leq l_j \leq r_j \leq n$, $1 \leq x_j \leq 5 \cdot 10^4$).</p><p>If $t_j = 2$, it is followed by two integers $l_j$ and $r_j$ ($1 \leq l_j \leq r_j \leq n$).</p><p>It is guaranteed that there is at least one query of type $2$.</p>

## Output

<p>For each query of the second type, output the minimum value of the expression.</p>





```input1|4,6,8,10,12
10 10
6 10 15 4 9 25 2 3 5 30
1 2 3 4 6 9 12 15 18 30
2 1 10
1 7 10 9
2 5 10
1 1 6 14
2 4 7
2 3 9
1 2 9 30
2 1 4
2 3 7
2 5 10
```




```input2|4,6
4 4
10 2 12 5
1 12 16 1
2 2 4
1 2 3 18
1 2 2 10
2 2 3
```




```output1
1
2
12
2
10
5
2
```




```output2
5
30
```



## Note

<p>In the first example:</p><ul><li> For the first query we can choose $i = 4$. So the value is $\frac{\operatorname{lcm}(4, 4)}{\gcd(4, 4)} = \frac{4}{4} = 1$.</li><li> After the second query the array $a = [6, 10, 15, 4, 9, 25, 9, 9, 9, 9]$.</li><li> For the third query we can choose $i = 9$. So the value is $\frac{\operatorname{lcm}(9, 18)}{\gcd(9, 18)} = \frac{18}{9} = 2$.</li></ul><p>In the second:</p><ul><li> For the first query we can choose $i = 4$. So the value is $\frac{\operatorname{lcm}(1, 5)}{\gcd(1, 5)} = \frac{5}{1} = 5$.</li><li> After the second query the array $a = [10, 18, 18, 5]$.</li><li> After the third query the array $a = [10, 10, 18, 5]$.</li><li> For the fourth query we can choose $i = 2$. So the value is $\frac{\operatorname{lcm}(10, 12)}{\gcd(10, 12)} = \frac{60}{2} = 30$. </li></ul>
