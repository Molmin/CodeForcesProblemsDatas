## Description

<div><p>Let's call <span class="tex-font-style-it">left cyclic shift</span> of some string $t_1 t_2 t_3 \dots t_{n - 1} t_n$ as string $t_2 t_3 \dots t_{n - 1} t_n t_1$.</p><p>Analogically, let's call <span class="tex-font-style-it">right cyclic shift</span> of string $t$ as string $t_n t_1 t_2 t_3 \dots t_{n - 1}$.</p><p>Let's say string $t$ is <span class="tex-font-style-bf">good</span> if its left cyclic shift is equal to its right cyclic shift.</p><p>You are given string $s$ which consists of digits <span class="tex-font-style-tt">0</span>–<span class="tex-font-style-tt">9</span>.</p><p>What is the minimum number of characters you need to erase from $s$ to make it good?</p></div><div class="input-specification"><p>The first line contains single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contains test cases&nbsp;— one per line. The first and only line of each test case contains string $s$ ($2 \le |s| \le 2 \cdot 10^5$). Each character $s_i$ is digit <span class="tex-font-style-tt">0</span>–<span class="tex-font-style-tt">9</span>.</p><p>It's guaranteed that the total length of strings doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum number of characters you need to erase from $s$ to make it good.</p></div>

## Input

<p>The first line contains single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contains test cases&nbsp;— one per line. The first and only line of each test case contains string $s$ ($2 \le |s| \le 2 \cdot 10^5$). Each character $s_i$ is digit <span class="tex-font-style-tt">0</span>–<span class="tex-font-style-tt">9</span>.</p><p>It's guaranteed that the total length of strings doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the minimum number of characters you need to erase from $s$ to make it good.</p>





```input1
3
95831
100120013
252525252525
```




```output1
3
5
0
```



## Note

<p>In the first test case, you can erase any $3$ characters, for example, the $1$-st, the $3$-rd, and the $4$-th. You'll get string <span class="tex-font-style-tt">51</span> and it is good.</p><p>In the second test case, we can erase all characters except <span class="tex-font-style-tt">0</span>: the remaining string is <span class="tex-font-style-tt">0000</span> and it's good.</p><p>In the third test case, the given string $s$ is already good.</p>
