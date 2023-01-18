## Description

<div><p>A <span class="tex-font-style-it">permutation</span> of length $k$ is a sequence of $k$ integers from $1$ to $k$ containing each integer exactly once. For example, the sequence $[3, 1, 2]$ is a permutation of length $3$.</p><p>When Neko was five, he thought of an array $a$ of $n$ positive integers and a permutation $p$ of length $n - 1$. Then, he performed the following:</p><ul> <li> Constructed an array $b$ of length $n-1$, where $b_i = \min(a_i, a_{i+1})$. </li><li> Constructed an array $c$ of length $n-1$, where $c_i = \max(a_i, a_{i+1})$. </li><li> Constructed an array $b'$ of length $n-1$, where $b'_i = b_{p_i}$. </li><li> Constructed an array $c'$ of length $n-1$, where $c'_i = c_{p_i}$. </li></ul><p>For example, if the array $a$ was $[3, 4, 6, 5, 7]$ and permutation $p$ was $[2, 4, 1, 3]$, then Neko would have constructed the following arrays:</p><ul> <li> $b = [3, 4, 5, 5]$ </li><li> $c = [4, 6, 6, 7]$ </li><li> $b' = [4, 5, 3, 5]$ </li><li> $c' = [6, 7, 4, 6]$ </li></ul><p>Then, he wrote two arrays $b'$ and $c'$ on a piece of paper and forgot about it. 14 years later, when he was cleaning up his room, he discovered this old piece of paper with two arrays $b'$ and $c'$ written on it. However he can't remember the array $a$ and permutation $p$ he used.</p><p>In case Neko made a mistake and there is no array $a$ and permutation $p$ resulting in such $b'$ and $c'$, print <span class="tex-font-style-tt">-1</span>. Otherwise, help him recover any possible array $a$. </p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of elements in array $a$.</p><p>The second line contains $n-1$ integers $b'_1, b'_2, \ldots, b'_{n-1}$ ($1 \leq b'_i \leq 10^9$).</p><p>The third line contains $n-1$ integers $c'_1, c'_2, \ldots, c'_{n-1}$ ($1 \leq c'_i \leq 10^9$).</p></div><div class="output-specification"><p>If Neko made a mistake and there is no array $a$ and a permutation $p$ leading to the $b'$ and $c'$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print $n$ positive integers $a_i$ ($1 \le a_i \le 10^9$), denoting the elements of the array $a$.</p><p>If there are multiple possible solutions, print any of them. </p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of elements in array $a$.</p><p>The second line contains $n-1$ integers $b'_1, b'_2, \ldots, b'_{n-1}$ ($1 \leq b'_i \leq 10^9$).</p><p>The third line contains $n-1$ integers $c'_1, c'_2, \ldots, c'_{n-1}$ ($1 \leq c'_i \leq 10^9$).</p>

## Output

<p>If Neko made a mistake and there is no array $a$ and a permutation $p$ leading to the $b'$ and $c'$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print $n$ positive integers $a_i$ ($1 \le a_i \le 10^9$), denoting the elements of the array $a$.</p><p>If there are multiple possible solutions, print any of them. </p>





```input1
5
4 5 3 5
6 7 4 6
```




```input2
3
2 4
3 2
```




```input3
8
2 3 1 1 2 4 3
3 4 4 2 5 5 4
```




```output1
3 4 6 5 7
```




```output2
-1
```




```output3
3 4 5 2 1 4 3 2
```



## Note

<p>The first example is explained is the problem statement.</p><p>In the third example, for $a = [3, 4, 5, 2, 1, 4, 3, 2]$, a possible permutation $p$ is $[7, 1, 5, 4, 3, 2, 6]$. In that case, Neko would have constructed the following arrays:</p><ul> <li> $b = [3, 4, 2, 1, 1, 3, 2]$ </li><li> $c = [4, 5, 5, 2, 4, 4, 3]$ </li><li> $b' = [2, 3, 1, 1, 2, 4, 3]$ </li><li> $c' = [3, 4, 4, 2, 5, 5, 4]$ </li></ul>
