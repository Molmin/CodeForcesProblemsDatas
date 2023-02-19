## Description

<div><p>You are given an array $a$ of length $n$. The array is called <span class="tex-font-style-it">3SUM-closed</span> if for all distinct indices $i$, $j$, $k$, the sum $a_i + a_j + a_k$ is an element of the array. More formally, $a$ is 3SUM-closed if for all integers $1 \leq i &lt; j &lt; k \leq n$, there exists some integer $1 \leq l \leq n$ such that $a_i + a_j + a_k = a_l$.</p><p>Determine if $a$ is 3SUM-closed.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $a$ is 3SUM-closed and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $a$ is 3SUM-closed and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,3,6,7
4
3
-1 0 1
5
1 -2 -2 1 -3
6
0 0 0 0 0 0
4
-1 2 -3 4
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first test case, there is only one triple where $i=1$, $j=2$, $k=3$. In this case, $a_1 + a_2 + a_3 = 0$, which is an element of the array ($a_2 = 0$), so the array is 3SUM-closed.</p><p>In the second test case, $a_1 + a_4 + a_5 = -1$, which is not an element of the array. Therefore, the array is not 3SUM-closed.</p><p>In the third test case, $a_i + a_j + a_k = 0$ for all distinct $i$, $j$, $k$, and $0$ is an element of the array, so the array is 3SUM-closed.</p>
