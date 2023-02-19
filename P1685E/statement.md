## Description

<div><p><span class="tex-font-style-it">It turns out that this is exactly the $100$-th problem of mine that appears in some programming competition. So it has to be special! And what can be more special than another problem about LIS...</span></p><p>You are given a permutation $p_1, p_2, \ldots, p_{2n+1}$ of integers from $1$ to $2n+1$. You will have to process $q$ updates, where the $i$-th update consists in swapping $p_{u_i}, p_{v_i}$.</p><p>After each update, find any cyclic shift of $p$ with $LIS \le n$, or determine that there is no such shift. (Refer to the output section for details).</p><p>Here $LIS(a)$ denotes the length of <a href="https://en.wikipedia.org/wiki/Longest_increasing_subsequence">longest strictly increasing subsequence</a> of $a$.</p><p><span class="tex-font-style-bf">Hacks are disabled in this problem. Don't ask why</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n, q$ ($2 \le n \le 10^5$, $1 \le q \le 10^5$).</p><p>The second line of the input contains $2n+1$ integers $p_1, p_2, \ldots, p_{2n+1}$ ($1 \le p_i \le 2n+1$, all $p_i$ are distinct) &nbsp;— the elements of $p$.</p><p>The $i$-th of the next $q$ lines contains two integers $u_i, v_i$ ($1 \le u_i, v_i \le 2n+1$, $u_i \neq v_i$) &nbsp;— indicating that you have to swap elements $p_{u_i}, p_{v_i}$ in the $i$-th update.</p></div><div class="output-specification"><p>After each update, output <span class="tex-font-style-bf">any</span> $k$ $(0 \le k \le 2n)$, such that the length of the longest increasing subsequence of $(p_{k+1}, p_{k+2}, \ldots, p_{2n+1}, p_1, \ldots, p_k)$ doesn't exceed $n$, or $-1$, if there is no such $k$.</p></div>

## Input

<p>The first line of the input contains two integers $n, q$ ($2 \le n \le 10^5$, $1 \le q \le 10^5$).</p><p>The second line of the input contains $2n+1$ integers $p_1, p_2, \ldots, p_{2n+1}$ ($1 \le p_i \le 2n+1$, all $p_i$ are distinct) &nbsp;— the elements of $p$.</p><p>The $i$-th of the next $q$ lines contains two integers $u_i, v_i$ ($1 \le u_i, v_i \le 2n+1$, $u_i \neq v_i$) &nbsp;— indicating that you have to swap elements $p_{u_i}, p_{v_i}$ in the $i$-th update.</p>

## Output

<p>After each update, output <span class="tex-font-style-bf">any</span> $k$ $(0 \le k \le 2n)$, such that the length of the longest increasing subsequence of $(p_{k+1}, p_{k+2}, \ldots, p_{2n+1}, p_1, \ldots, p_k)$ doesn't exceed $n$, or $-1$, if there is no such $k$.</p>





```input1
2 6
1 2 3 4 5
1 5
1 5
4 5
5 4
1 4
2 5
```




```output1
-1
-1
2
-1
4
0
```



## Note

<p>After the first update, our permutation becomes $(5, 2, 3, 4, 1)$. We can show that all its cyclic shifts have $LIS \ge 3$.</p><p>After the second update, our permutation becomes $(1, 2, 3, 4, 5)$. We can show that all its cyclic shifts have $LIS \ge 3$.</p><p>After the third update, our permutation becomes $(1, 2, 3, 5, 4)$. Its shift by $2$ is $(3, 5, 4, 1, 2)$, and its $LIS = 2$.</p><p>After the fourth update, our permutation becomes $(1, 2, 3, 4, 5)$. We can show that all its cyclic shifts have $LIS \ge 3$.</p><p>After the fifth update, our permutation becomes $(4, 2, 3, 1, 5)$. Its shift by $4$ is $(5, 4, 2, 3, 1)$, and its $LIS = 2$.</p><p>After the fifth update, our permutation becomes $(4, 5, 3, 1, 2)$. Its shift by $0$ is $(4, 5, 3, 1, 2)$, and its $LIS = 2$.</p>
