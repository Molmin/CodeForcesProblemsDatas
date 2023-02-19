## Description

<div><p>Let's call a list of positive integers $a_0, a_1, ..., a_{n-1}$ a <span class="tex-font-style-bf">power sequence</span> if there is a positive integer $c$, so that for every $0 \le i \le n-1$ then $a_i = c^i$.</p><p>Given a list of $n$ positive integers $a_0, a_1, ..., a_{n-1}$, you are allowed to:</p><ul> <li> Reorder the list (i.e. pick a permutation $p$ of $\{0,1,...,n - 1\}$ and change $a_i$ to $a_{p_i}$), then </li><li> Do the following operation any number of times: pick an index $i$ and change $a_i$ to $a_i - 1$ or $a_i + 1$ (i.e. increment or decrement $a_i$ by $1$) with a cost of $1$. </li></ul><p>Find the minimum cost to transform $a_0, a_1, ..., a_{n-1}$ into a power sequence.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_0, a_1, ..., a_{n-1}$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Print the minimum cost to transform $a_0, a_1, ..., a_{n-1}$ into a power sequence.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_0, a_1, ..., a_{n-1}$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>Print the minimum cost to transform $a_0, a_1, ..., a_{n-1}$ into a power sequence.</p>





```input1
3
1 3 2
```




```input2
3
1000000000 1000000000 1000000000
```




```output1
1
```




```output2
1999982505
```



## Note

<p>In the first example, we first reorder $\{1, 3, 2\}$ into $\{1, 2, 3\}$, then increment $a_2$ to $4$ with cost $1$ to get a power sequence $\{1, 2, 4\}$.</p>
