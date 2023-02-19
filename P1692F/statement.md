## Description

<div><p>Given an array $a$ of positive integers with length $n$, determine if there exist three <span class="tex-font-style-bf">distinct</span> indices $i$, $j$, $k$ such that $a_i + a_j + a_k$ ends in the digit $3$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $t$ lines, each of which contains the answer to the corresponding test case. Output "<span class="tex-font-style-tt">YES</span>" if there exist three <span class="tex-font-style-bf">distinct</span> indices $i$, $j$, $k$ satisfying the constraints in the statement, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $t$ lines, each of which contains the answer to the corresponding test case. Output "<span class="tex-font-style-tt">YES</span>" if there exist three <span class="tex-font-style-bf">distinct</span> indices $i$, $j$, $k$ satisfying the constraints in the statement, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1
6
4
20 22 19 84
4
1 11 1 2022
4
1100 1100 1100 1111
5
12 34 56 78 90
4
1 9 8 4
6
16 38 94 25 18 99
```




```output1
YES
YES
NO
NO
YES
YES
```



## Note

<p>In the first test case, you can select $i=1$, $j=4$, $k=3$. Then $a_1 + a_4 + a_3 = 20 + 84 + 19 = 123$, which ends in the digit $3$.</p><p>In the second test case, you can select $i=1$, $j=2$, $k=3$. Then $a_1 + a_2 + a_3 = 1 + 11 + 1 = 13$, which ends in the digit $3$.</p><p>In the third test case, it can be proven that no such $i$, $j$, $k$ exist. Note that $i=4$, $j=4$, $k=4$ is <span class="tex-font-style-bf">not</span> a valid solution, since although $a_4 + a_4 + a_4 = 1111 + 1111 + 1111 = 3333$, which ends in the digit $3$, the indices need to be <span class="tex-font-style-bf">distinct</span>.</p><p>In the fourth test case, it can be proven that no such $i$, $j$, $k$ exist.</p><p>In the fifth test case, you can select $i=4$, $j=3$, $k=1$. Then $a_4 + a_3 + a_1 = 4 + 8 + 1 = 13$, which ends in the digit $3$.</p><p>In the sixth test case, you can select $i=1$, $j=2$, $k=6$. Then $a_1 + a_2 + a_6 = 16 + 38 + 99 = 153$, which ends in the digit $3$.</p>
