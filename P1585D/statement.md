## Description

<div><p>Petya has an array of integers $a_1, a_2, \ldots, a_n$. He only likes sorted arrays. Unfortunately, the given array could be arbitrary, so Petya wants to sort it.</p><p>Petya likes to challenge himself, so he wants to sort array using only $3$-cycles. More formally, in one operation he can pick $3$ <span class="tex-font-style-bf">pairwise distinct</span> indices $i$, $j$, and $k$ ($1 \leq i, j, k \leq n$) and apply $i \to j \to k \to i$ cycle to the array $a$. It simultaneously places $a_i$ on position $j$, $a_j$ on position $k$, and $a_k$ on position $i$, without changing any other element.</p><p>For example, if $a$ is $[10, 50, 20, 30, 40, 60]$ and he chooses $i = 2$, $j = 1$, $k = 5$, then the array becomes $[\underline{50}, \underline{40}, 20, 30, \underline{10}, 60]$.</p><p>Petya can apply arbitrary number of $3$-cycles (possibly, zero). You are to determine if Petya can sort his array $a$, i.&nbsp;e. make it non-decreasing.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 5 \cdot 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if Petya can sort the array $a$ using $3$-cycles, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 5 \cdot 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if Petya can sort the array $a$ using $3$-cycles, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can print each letter in any case (upper or lower).</p>





```input1
7
1
1
2
2 2
2
2 1
3
1 2 3
3
2 1 3
3
3 1 2
4
2 1 4 3
```




```output1
YES
YES
NO
YES
NO
YES
YES
```



## Note

<p>In the $6$-th test case Petya can use the $3$-cycle $1 \to 3 \to 2 \to 1$ to sort the array.</p><p>In the $7$-th test case Petya can apply $1 \to 3 \to 2 \to 1$ and make $a = [1, 4, 2, 3]$. Then he can apply $2 \to 4 \to 3 \to 2$ and finally sort the array.</p>
