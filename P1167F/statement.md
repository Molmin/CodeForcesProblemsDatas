## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$. All $a_i$ are pairwise distinct.</p><p>Let's define function $f(l, r)$ as follows: </p><ul> <li> let's define array $b_1, b_2, \dots, b_{r - l + 1}$, where $b_i = a_{l - 1 + i}$; </li><li> sort array $b$ in increasing order; </li><li> result of the function $f(l, r)$ is $\sum\limits_{i = 1}^{r - l + 1}{b_i \cdot i}$. </li></ul><p>Calculate $\left(\sum\limits_{1 \le l \le r \le n}{f(l, r)}\right) \mod (10^9+7)$, i.e. total sum of $f$ for all subsegments of $a$ modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the length of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$, $a_i \neq a_j$ for $i \neq j$) — array $a$.</p></div><div class="output-specification"><p>Print one integer — the total sum of $f$ for all subsegments of $a$ modulo $10^9+7$</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the length of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$, $a_i \neq a_j$ for $i \neq j$) — array $a$.</p>

## Output

<p>Print one integer — the total sum of $f$ for all subsegments of $a$ modulo $10^9+7$</p>





```input1
4
5 2 4 7
```




```input2
3
123456789 214365879 987654321
```




```output1
167
```




```output2
582491518
```



## Note

<p>Description of the first example: </p><ul> <li> $f(1, 1) = 5 \cdot 1 = 5$; </li><li> $f(1, 2) = 2 \cdot 1 + 5 \cdot 2 = 12$; </li><li> $f(1, 3) = 2 \cdot 1 + 4 \cdot 2 + 5 \cdot 3 = 25$; </li><li> $f(1, 4) = 2 \cdot 1 + 4 \cdot 2 + 5 \cdot 3 + 7 \cdot 4 = 53$; </li><li> $f(2, 2) = 2 \cdot 1 = 2$; </li><li> $f(2, 3) = 2 \cdot 1 + 4 \cdot 2 = 10$; </li><li> $f(2, 4) = 2 \cdot 1 + 4 \cdot 2 + 7 \cdot 3 = 31$; </li><li> $f(3, 3) = 4 \cdot 1 = 4$; </li><li> $f(3, 4) = 4 \cdot 1 + 7 \cdot 2 = 18$; </li><li> $f(4, 4) = 7 \cdot 1 = 7$; </li></ul>
