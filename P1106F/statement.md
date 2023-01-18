## Description

<div><p><span class="tex-font-style-it">Lunar New Year is approaching, and Bob received a gift from his friend recently — a recursive sequence!</span> He loves this sequence very much and wants to play with it.</p><p>Let $f_1, f_2, \ldots, f_i, \ldots$ be an infinite sequence of positive integers. Bob knows that for $i &gt; k$, $f_i$ can be obtained by the following recursive equation:</p><p>$$f_i = \left(f_{i - 1} ^ {b_1} \cdot f_{i - 2} ^ {b_2} \cdot \cdots \cdot f_{i - k} ^ {b_k}\right) \bmod p,$$</p><p>which in short is</p><p>$$f_i = \left(\prod_{j = 1}^{k} f_{i - j}^{b_j}\right) \bmod p,$$</p><p>where $p = 998\,244\,353$ (a widely-used prime), $b_1, b_2, \ldots, b_k$ are known integer constants, and $x \bmod y$ denotes the remainder of $x$ divided by $y$.</p><p>Bob lost the values of $f_1, f_2, \ldots, f_k$, which is extremely troublesome – these are the basis of the sequence! Luckily, Bob remembers the first $k - 1$ elements of the sequence: $f_1 = f_2 = \ldots = f_{k - 1} = 1$ and the $n$-th element: $f_n = m$. Please find any possible value of $f_k$. If no solution exists, just tell Bob that it is impossible to recover his favorite sequence, regardless of Bob's sadness.</p></div><div class="input-specification"><p>The first line contains a positive integer $k$ ($1 \leq k \leq 100$), denoting the length of the sequence $b_1, b_2, \ldots, b_k$.</p><p>The second line contains $k$ positive integers $b_1, b_2, \ldots, b_k$ ($1 \leq b_i &lt; p$).</p><p>The third line contains two positive integers $n$ and $m$ ($k &lt; n \leq 10^9$, $1 \leq m &lt; p$), which implies $f_n = m$.</p></div><div class="output-specification"><p>Output a possible value of $f_k$, where $f_k$ is a positive integer satisfying $1 \leq f_k &lt; p$. If there are multiple answers, print any of them. If no such $f_k$ makes $f_n = m$, output $-1$ instead.</p><p>It is easy to show that if there are some possible values of $f_k$, there must be at least one satisfying $1 \leq f_k &lt; p$.</p></div>

## Input

<p>The first line contains a positive integer $k$ ($1 \leq k \leq 100$), denoting the length of the sequence $b_1, b_2, \ldots, b_k$.</p><p>The second line contains $k$ positive integers $b_1, b_2, \ldots, b_k$ ($1 \leq b_i &lt; p$).</p><p>The third line contains two positive integers $n$ and $m$ ($k &lt; n \leq 10^9$, $1 \leq m &lt; p$), which implies $f_n = m$.</p>

## Output

<p>Output a possible value of $f_k$, where $f_k$ is a positive integer satisfying $1 \leq f_k &lt; p$. If there are multiple answers, print any of them. If no such $f_k$ makes $f_n = m$, output $-1$ instead.</p><p>It is easy to show that if there are some possible values of $f_k$, there must be at least one satisfying $1 \leq f_k &lt; p$.</p>





```input1
3
2 3 5
4 16
```




```input2
5
4 7 1 5 6
7 14187219
```




```input3
8
2 3 5 6 1 7 9 10
23333 1
```




```input4
1
2
88888 66666
```




```input5
3
998244352 998244352 998244352
4 2
```




```input6
10
283 463 213 777 346 201 463 283 102 999
2333333 6263423
```




```output1
4
```




```output2
6
```




```output3
1
```




```output4
-1
```




```output5
-1
```




```output6
382480067
```



## Note

<p>In the first sample, we have $f_4 = f_3^2 \cdot f_2^3 \cdot f_1^5$. Therefore, applying $f_3 = 4$, we have $f_4 = 16$. Note that there can be multiple answers.</p><p>In the third sample, applying $f_7 = 1$ makes $f_{23333} = 1$.</p><p>In the fourth sample, no such $f_1$ makes $f_{88888} = 66666$. Therefore, we output $-1$ instead.</p>
