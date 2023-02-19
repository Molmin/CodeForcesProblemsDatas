## Description

<div><p>We call an array $a$ <span class="tex-font-style-it">pure</span> if all elements in it are pairwise distinct. For example, an array $[1, 7, 9]$ is pure, $[1, 3, 3, 7]$ isn't, because $3$ occurs twice in it.</p><p>A pure array $b$ is <span class="tex-font-style-it">similar</span> to a pure array $c$ if their lengths $n$ are the same and for all pairs of indices $l$, $r$, such that $1 \le l \le r \le n$, it's true that $$\operatorname{argmax}([b_l, b_{l + 1}, \ldots, b_r]) = \operatorname{argmax}([c_l, c_{l + 1}, \ldots, c_r]),$$ where $\operatorname{argmax}(x)$ is defined as the index of the largest element in $x$ (which is unique for pure arrays). For example, $\operatorname{argmax}([3, 4, 2]) = 2$, $\operatorname{argmax}([1337, 179, 57]) = 1$.</p><p>Recently, Tonya found out that Burenka really likes a permutation $p$ of length $n$. Tonya decided to please her and give her an array $a$ <span class="tex-font-style-it">similar</span> to $p$. He already fixed some elements of $a$, but exactly $k$ elements are missing (in these positions temporarily $a_i = 0$). It is guaranteed that $k \ge 2$. Also, he has a set $S$ of $k - 1$ numbers.</p><p>Tonya realized that he was missing one number to fill the empty places of $a$, so he decided to buy it. He has $q$ options to buy. Tonya thinks that the number $d$ suits him, if it is possible to replace all zeros in $a$ with numbers from $S$ and the number $d$, so that $a$ becomes a <span class="tex-font-style-it">pure</span> array <span class="tex-font-style-it">similar</span> to $p$. For each option of $d$, output whether this number is suitable for him or not.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) is the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a couple of integers $n$ and $q$ ($1 \le n, q \le 3 \cdot 10^5$).</p><p>The second line of each input test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$)&nbsp;— the permutation Burenka likes.</p><p>The third line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^6$)&nbsp;— elements of Tonya's array, where $0$ denotes a missing element. It is guaranteed that there are two indexes $i, j$ $(1 \le i, j \le n, i \ne j)$ such that $a_i = 0, a_j = 0$, which implies that $k \geq 2$.</p><p>The fourth line of each test case contains $k - 1$ distinct integers $s_1, s_2, \ldots, s_{k-1}$ ($1 \le s_i \le 10^6$)&nbsp;— elements of Tonya's set $S$.</p><p>Each of the next $q$ lines contains a single integer $d$ ($1 \le d \le 10^6$)&nbsp;— the number that Tonya plans to buy.</p><p>It is guaranteed that for each given $d$ it's <span class="tex-font-style-bf">possible</span> to fill in the gaps in $a$ with numbers from $S$ and the number $d$ to get a pure array.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ in all tests does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $q$ lines. For each value $d$, print "<span class="tex-font-style-tt">YES</span>" if there is a way to fill the array $a$ to make it similar to $p$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) is the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a couple of integers $n$ and $q$ ($1 \le n, q \le 3 \cdot 10^5$).</p><p>The second line of each input test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$)&nbsp;— the permutation Burenka likes.</p><p>The third line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^6$)&nbsp;— elements of Tonya's array, where $0$ denotes a missing element. It is guaranteed that there are two indexes $i, j$ $(1 \le i, j \le n, i \ne j)$ such that $a_i = 0, a_j = 0$, which implies that $k \geq 2$.</p><p>The fourth line of each test case contains $k - 1$ distinct integers $s_1, s_2, \ldots, s_{k-1}$ ($1 \le s_i \le 10^6$)&nbsp;— elements of Tonya's set $S$.</p><p>Each of the next $q$ lines contains a single integer $d$ ($1 \le d \le 10^6$)&nbsp;— the number that Tonya plans to buy.</p><p>It is guaranteed that for each given $d$ it's <span class="tex-font-style-bf">possible</span> to fill in the gaps in $a$ with numbers from $S$ and the number $d$ to get a pure array.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ in all tests does not exceed $3 \cdot 10^5$.</p>

## Output

<p>Output $q$ lines. For each value $d$, print "<span class="tex-font-style-tt">YES</span>" if there is a way to fill the array $a$ to make it similar to $p$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1|2,3,4,5,6,7,8,16,17,18,19,20,21
4
4 3
1 4 3 2
5 0 7 0
6
9
1
4
5 3
1 2 5 4 3
0 5 10 0 0
3 9
1
8
11
5 2
1 4 3 2 5
0 0 0 0 0
7 9 1 5
6
100
4 2
4 1 3 2
0 5 3 0
2
4
6
```




```output1
YES
NO
NO
YES
YES
NO
YES
YES
NO
NO
```



## Note

<p>In the first test case for $d = 9$, you can get $a = [5, 9, 7, 6]$, it can be proved that $a$ is similar to $p$, for $d=1$ and $d=4$ it can be proved that there is no answer.</p><p>In the second test case for $d = 1$, you can get $a = [1, 5, 10, 9, 3]$, for $d = 8$, you can get $a = [3, 5, 10, 9, 8]$, it can be proved that for $d = 11$ there is no answer.</p>
