## Description

<div><p>You are given a permutation $p_1, p_2, \dots , p_n$ (an array where each integer from $1$ to $n$ appears exactly once). The weight of the $i$-th element of this permutation is $a_i$.</p><p>At first, you separate your permutation into two <span class="tex-font-style-bf">non-empty</span> sets — prefix and suffix. More formally, the first set contains elements $p_1, p_2, \dots , p_k$, the second — $p_{k+1}, p_{k+2}, \dots , p_n$, where $1 \le k &lt; n$.</p><p>After that, you may move elements between sets. The operation you are allowed to do is to choose some element of the first set and move it to the second set, or vice versa (move from the second set to the first). You have to pay $a_i$ dollars to move the element $p_i$.</p><p>Your goal is to make it so that each element of the first set is less than each element of the second set. Note that if one of the sets is empty, this condition is met.</p><p>For example, if $p = [3, 1, 2]$ and $a = [7, 1, 4]$, then the optimal strategy is: separate $p$ into two parts $[3, 1]$ and $[2]$ and then move the $2$-element into first set (it costs $4$). And if $p = [3, 5, 1, 6, 2, 4]$, $a = [9, 1, 9, 9, 1, 9]$, then the optimal strategy is: separate $p$ into two parts $[3, 5, 1]$ and $[6, 2, 4]$, and then move the $2$-element into first set (it costs $1$), and $5$-element into second set (it also costs $1$).</p><p>Calculate the minimum number of dollars you have to spend.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of permutation.</p><p>The second line contains $n$ integers $p_1, p_2, \dots , p_n$ ($1 \le p_i \le n$). It's guaranteed that this sequence contains each element from $1$ to $n$ exactly once.</p><p>The third line contains $n$ integers $a_1, a_2, \dots , a_n$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Print one integer — the minimum number of dollars you have to spend.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of permutation.</p><p>The second line contains $n$ integers $p_1, p_2, \dots , p_n$ ($1 \le p_i \le n$). It's guaranteed that this sequence contains each element from $1$ to $n$ exactly once.</p><p>The third line contains $n$ integers $a_1, a_2, \dots , a_n$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>Print one integer — the minimum number of dollars you have to spend.</p>





```input1
3
3 1 2
7 1 4
```




```input2
4
2 4 1 3
5 9 8 3
```




```input3
6
3 5 1 6 2 4
9 1 9 9 1 9
```




```output1
4
```




```output2
3
```




```output3
2
```


