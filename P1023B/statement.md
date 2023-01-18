## Description

<div><p>Tanechka is shopping in the toy shop. There are exactly $n$ toys in the shop for sale, the cost of the $i$-th toy is $i$ burles. She wants to choose two toys in such a way that their total cost is $k$ burles. How many ways to do that does she have?</p><p>Each toy appears in the shop exactly once. Pairs $(a, b)$ and $(b, a)$ are considered equal. Pairs $(a, b)$, where $a=b$, are not allowed.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$, $k$ ($1 \le n, k \le 10^{14}$) — the number of toys and the expected total cost of the pair of toys.</p></div><div class="output-specification"><p>Print the number of ways to choose the pair of toys satisfying the condition above. Print <span class="tex-font-style-tt">0</span>, if Tanechka can choose no pair of toys in such a way that their total cost is $k$ burles.</p></div>

## Input

<p>The first line of the input contains two integers $n$, $k$ ($1 \le n, k \le 10^{14}$) — the number of toys and the expected total cost of the pair of toys.</p>

## Output

<p>Print the number of ways to choose the pair of toys satisfying the condition above. Print <span class="tex-font-style-tt">0</span>, if Tanechka can choose no pair of toys in such a way that their total cost is $k$ burles.</p>





```input1
8 5

```




```input2
8 15

```




```input3
7 20

```




```input4
1000000000000 1000000000001

```




```output1
2

```




```output2
1

```




```output3
0

```




```output4
500000000000

```



## Note

<p>In the first example Tanechka can choose the pair of toys ($1, 4$) or the pair of toys ($2, 3$).</p><p>In the second example Tanechka can choose only the pair of toys ($7, 8$).</p><p>In the third example choosing any pair of toys will lead to the total cost less than $20$. So the answer is <span class="tex-font-style-tt">0</span>.</p><p>In the fourth example she can choose the following pairs: $(1, 1000000000000)$, $(2, 999999999999)$, $(3, 999999999998)$, ..., $(500000000000, 500000000001)$. The number of such pairs is exactly $500000000000$.</p>
