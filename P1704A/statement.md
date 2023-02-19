## Description

<div><p>AquaMoon has two binary sequences $a$ and $b$, which contain only $0$ and $1$. AquaMoon can perform the following two operations any number of times ($a_1$ is the first element of $a$, $a_2$ is the second element of $a$, and so on):</p><ul><li> <span class="tex-font-style-it">Operation 1</span>: if $a$ contains at least two elements, change $a_2$ to $\operatorname{min}(a_1,a_2)$, and remove the first element of $a$.</li><li> <span class="tex-font-style-it">Operation 2</span>: if $a$ contains at least two elements, change $a_2$ to $\operatorname{max}(a_1,a_2)$, and remove the first element of $a$.</li></ul><p>Note that after a removal of the first element of $a$, the former $a_2$ becomes the first element of $a$, the former $a_3$ becomes the second element of $a$ and so on, and the length of $a$ reduces by one.</p><p>Determine if AquaMoon can make $a$ equal to $b$ by using these operations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 2\,000$) — the number of test cases. Description of test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ ($1 \leq n,m \leq 50$, $m \leq n$) — the lengths of $a$ and $b$ respectively.</p><p>The second line of each test case contains a string $a$ of length $n$, consisting only $0$ and $1$.</p><p>The third line of each test case contains a string $b$ of length $m$, consisting only $0$ and $1$.</p></div><div class="output-specification"><p>For each test case, output "YES" if AquaMoon can change $a$ to $b$ by using these options; otherwise, output "NO".</p><p>You may print each letter in any case (for example, "YES", "Yes", "yes", "yEs" will all be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 2\,000$) — the number of test cases. Description of test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ ($1 \leq n,m \leq 50$, $m \leq n$) — the lengths of $a$ and $b$ respectively.</p><p>The second line of each test case contains a string $a$ of length $n$, consisting only $0$ and $1$.</p><p>The third line of each test case contains a string $b$ of length $m$, consisting only $0$ and $1$.</p>

## Output

<p>For each test case, output "YES" if AquaMoon can change $a$ to $b$ by using these options; otherwise, output "NO".</p><p>You may print each letter in any case (for example, "YES", "Yes", "yes", "yEs" will all be recognized as a positive answer).</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22,26,27,28
10
6 2
001001
11
6 2
110111
01
6 2
000001
11
6 2
111111
01
8 5
10000101
11010
7 4
1010001
1001
8 6
01010010
010010
8 4
01010101
1001
8 4
10101010
0110
7 5
1011100
11100
```




```output1
YES
YES
NO
NO
NO
YES
YES
NO
NO
YES
```



## Note

<p>In the first test case, you can use <span class="tex-font-style-it">Operation 2</span> four times to make $a$ equals to $b$.</p><p>In the second test case, you can use <span class="tex-font-style-it">Operation 1</span> four times to make $a$ equals to $b$.</p><p>In the third test case, it can be proved that no matter how we use the operations, it is impossible to make $a$ equal to $b$.</p><p>In the fourth test case, it can be proved that no matter how we use the operations, it is impossible to make $a$ equal to $b$.</p><p>In the fifth test case, you can use <span class="tex-font-style-it">Operation 2</span> three times to make $a$ become $10101$, so the first element of $a$ equals to the first element of $b$, but it can be proved that no matter how to operate, the second to the fifth elements of $a$ can't be the same as $b$.</p>
