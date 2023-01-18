## Description

<div><p>You are given a permutation $p$ of $n$ integers $1$, $2$, ..., $n$ (a permutation is an array where each element from $1$ to $n$ occurs exactly once).</p><p>Let's call some subsegment $p[l, r]$ of this permutation special if $p_l + p_r = \max \limits_{i = l}^{r} p_i$. Please calculate the number of special subsegments.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($3 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $p_1$, $p_2$, ..., $p_n$ ($1 \le p_i \le n$). All these integers are pairwise distinct.</p></div><div class="output-specification"><p>Print the number of special subsegments of the given permutation.</p></div>

## Input

<p>The first line contains one integer $n$ ($3 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $p_1$, $p_2$, ..., $p_n$ ($1 \le p_i \le n$). All these integers are pairwise distinct.</p>

## Output

<p>Print the number of special subsegments of the given permutation.</p>





```input1
5
3 4 1 5 2
```




```input2
3
1 3 2
```




```output1
2
```




```output2
1
```



## Note

<p>Special subsegments in the first example are $[1, 5]$ and $[1, 3]$.</p><p>The only special subsegment in the second example is $[1, 3]$.</p>
