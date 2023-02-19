## Description

<div><p>You are given <span class="tex-font-style-bf">three</span> bags. Each bag contains a non-empty multiset of numbers. You can perform a number of operations on these bags. In one operation, you can choose any two non-empty bags, and choose one number from each of the bags. Let's say that you choose number $a$ from the first bag and number $b$ from the second bag. Then, you remove $b$ from the second bag and replace $a$ with $a-b$ in the first bag. Note that if there are multiple occurrences of these numbers, then you shall only remove/replace exactly one occurrence.</p><p>You have to perform these operations in such a way that you have exactly one number remaining in exactly one of the bags (the other two bags being empty). It can be shown that you can always apply these operations to receive such a configuration in the end. Among all these configurations, find the one which has the maximum number left in the end.</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers $n_1$, $n_2$ and $n_3$ ($1 \le n_1, n_2, n_3 \le 3\cdot10^5$, $1 \le n_1+n_2+n_3 \le 3\cdot10^5$) — the number of numbers in the three bags.</p><p>The $i$-th of the next three lines contain $n_i$ space-separated integers $a_{{i,1}}$, $a_{{i,2}}$, ..., $a_{{i,{{n_i}}}}$ ($1 \le a_{{i,j}} \le 10^9$) — the numbers in the $i$-th bag.</p></div><div class="output-specification"><p>Print a single integer — the maximum number which you can achieve in the end.</p></div>

## Input

<p>The first line of the input contains three space-separated integers $n_1$, $n_2$ and $n_3$ ($1 \le n_1, n_2, n_3 \le 3\cdot10^5$, $1 \le n_1+n_2+n_3 \le 3\cdot10^5$) — the number of numbers in the three bags.</p><p>The $i$-th of the next three lines contain $n_i$ space-separated integers $a_{{i,1}}$, $a_{{i,2}}$, ..., $a_{{i,{{n_i}}}}$ ($1 \le a_{{i,j}} \le 10^9$) — the numbers in the $i$-th bag.</p>

## Output

<p>Print a single integer — the maximum number which you can achieve in the end.</p>





```input1
2 4 1
1 2
6 3 4 5
5
```




```input2
3 2 2
7 5 4
2 9
7 1
```




```output1
20
```




```output2
29
```



## Note

<p>In the first example input, let us perform the following operations:</p><p>$[1, 2], [6, 3, 4, 5], [5]$</p><p>$[-5, 2], [3, 4, 5], [5]$ (Applying an operation to $(1, 6)$)</p><p>$[-10, 2], [3, 4], [5]$ (Applying an operation to $(-5, 5)$)</p><p>$[2], [3, 4], [15]$ (Applying an operation to $(5, -10)$)</p><p>$[-1], [4], [15]$ (Applying an operation to $(2, 3)$)</p><p>$[-5], [], [15]$ (Applying an operation to $(-1, 4)$)</p><p>$[], [], [20]$ (Applying an operation to $(15, -5)$)</p><p>You can verify that you cannot achieve a bigger number. Hence, the answer is $20$.</p>
