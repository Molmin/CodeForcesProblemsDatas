## Description

<div><p>You are given three integers $a$, $b$, and $c$. Determine if one of them is the sum of the other two.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 9261$)&nbsp;— the number of test cases.</p><p>The description of each test case consists of three integers $a$, $b$, $c$ ($0 \leq a, b, c \leq 20$).</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if one of the numbers is the sum of the other two, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 9261$)&nbsp;— the number of test cases.</p><p>The description of each test case consists of three integers $a$, $b$, $c$ ($0 \leq a, b, c \leq 20$).</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if one of the numbers is the sum of the other two, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,4,6,8
7
1 4 3
2 5 8
9 11 20
0 0 0
20 20 20
4 12 3
15 7 8
```




```output1
YES
NO
YES
YES
NO
NO
YES
```



## Note

<p>In the first test case, $1 + 3 = 4$.</p><p>In the second test case, none of the numbers is the sum of the other two.</p><p>In the third test case, $9 + 11 = 20$.</p>
