## Description

<div><p>You are given a permutation $p$ of length $n$, an array of $m$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_m$ ($1 \le a_i \le n$), and an integer $d$.</p><p>Let $\mathrm{pos}(x)$ be the index of $x$ in the permutation $p$. The array $a$ is <span class="tex-font-style-bf">not <span class="tex-font-style-it">good</span></span> if </p><ul> <li> $\mathrm{pos}(a_{i}) &lt; \mathrm{pos}(a_{i + 1}) \le \mathrm{pos}(a_{i}) + d$ for all $1 \le i &lt; m$. </li></ul><p>For example, with the permutation $p = [4, 2, 1, 3, 6, 5]$ and $d = 2$: </p><ul> <li> $a = [2, 3, 6]$ is a not <span class="tex-font-style-it">good</span> array. </li><li> $a = [2, 6, 5]$ is <span class="tex-font-style-it">good</span> because $\mathrm{pos}(a_1) = 2$, $\mathrm{pos}(a_2) = 5$, so the condition $\mathrm{pos}(a_2) \le \mathrm{pos}(a_1) + d$ is not satisfied. </li><li> $a = [1, 6, 3]$ is <span class="tex-font-style-it">good</span> because $\mathrm{pos}(a_2) = 5$, $\mathrm{pos}(a_3) = 4$, so the condition $\mathrm{pos}(a_2) &lt; \mathrm{pos}(a_3)$ is not satisfied. </li></ul><p>In one move, you can swap two adjacent elements of the permutation $p$. What is the minimum number of moves needed such that the array $a$ becomes <span class="tex-font-style-it">good</span>? It can be shown that there always exists a sequence of moves so that the array $a$ becomes <span class="tex-font-style-it">good</span>.</p><p>A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$, but there is $4$ in the array).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$ and $d$ ($2\leq n \leq 10^5$, $2\leq m\leq n$, $1 \le d \le n$), the length of the permutation $p$, the length of the array $a$ and the value of $d$. </p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1\leq p_i \leq n$, $p_i \ne p_j$ for $i \ne j$). </p><p>The third line contains $m$ distinct integers $a_1, a_2, \ldots, a_m$ ($1\leq a_i \leq n$, $a_i \ne a_j$ for $i \ne j$).</p><p>The sum of $n$ over all test cases doesn't exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum number of moves needed such that the array $a$ becomes <span class="tex-font-style-it">good</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$ and $d$ ($2\leq n \leq 10^5$, $2\leq m\leq n$, $1 \le d \le n$), the length of the permutation $p$, the length of the array $a$ and the value of $d$. </p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1\leq p_i \leq n$, $p_i \ne p_j$ for $i \ne j$). </p><p>The third line contains $m$ distinct integers $a_1, a_2, \ldots, a_m$ ($1\leq a_i \leq n$, $a_i \ne a_j$ for $i \ne j$).</p><p>The sum of $n$ over all test cases doesn't exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print the minimum number of moves needed such that the array $a$ becomes <span class="tex-font-style-it">good</span>.</p>





```input1|2,3,4,8,9,10,14,15,16
5
4 2 2
1 2 3 4
1 3
5 2 4
5 4 3 2 1
5 2
5 3 3
3 4 1 5 2
3 1 2
2 2 1
1 2
2 1
6 2 4
1 2 3 4 5 6
2 5
```




```output1
1
3
2
0
2
```



## Note

<p>In the first case, $pos(a_1)=1$, $pos(a_2)=3$. To make the array <span class="tex-font-style-it">good</span>, one way is to swap $p_3$ and $p_4$. After that, the array $a$ will be <span class="tex-font-style-it">good</span> because the condition $\mathrm{pos}(a_2) \le \mathrm{pos}(a_1) + d$ won't be satisfied.</p><p>In the second case, $pos(a_1)=1$, $pos(a_2)=4$. The $3$ moves could be: </p><ol> <li> Swap $p_3$ and $p_4$. </li><li> Swap $p_2$ and $p_3$. </li><li> Swap $p_1$ and $p_2$. </li></ol> After these moves, the permutation $p$ will be $[2,5,4,3,1]$. The array $a$ will be <span class="tex-font-style-it">good</span> because the condition $\mathrm{pos}(a_1) &lt; \mathrm{pos}(a_2)$ won't be satisfied. It can be shown that you can't make the array $a$ <span class="tex-font-style-it">good</span> with fewer moves.<p>In the third case, $pos(a_1)=1$, $pos(a_2)=3$, $pos(a_3)=5$. The $2$ moves can be: </p><ol> <li> Swap $p_4$ and $p_5$. </li><li> Swap $p_3$ and $p_4$. </li></ol> After these moves, the permutation $p$ will be $[3,4,2,1,5]$. The array $a$ will be <span class="tex-font-style-it">good</span> because the condition $\mathrm{pos}(a_2) &lt; \mathrm{pos}(a_3)$ won't be satisfied. It can be shown that you can't make the array $a$ <span class="tex-font-style-it">good</span> with fewer moves.<p>In the fourth case, $pos(a_1)=2$, $pos(a_2)=1$. The array $a$ is already <span class="tex-font-style-it">good</span>.</p><p>In the fifth case, $pos(a_1)=2$, $pos(a_2)=5$. The $2$ moves are: </p><ol> <li> Swap $p_1$ and $p_2$. </li><li> Swap $p_5$ and $p_6$. </li></ol>
