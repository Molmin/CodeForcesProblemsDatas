## Description

<div><p>You are given a string $s$ of length $n$ consisting of characters <span class="tex-font-style-tt">a</span> and/or <span class="tex-font-style-tt">b</span>.</p><p>Let $\operatorname{AB}(s)$ be the number of occurrences of string <span class="tex-font-style-tt">ab</span> in $s$ as a <span class="tex-font-style-bf">substring</span>. Analogically, $\operatorname{BA}(s)$ is the number of occurrences of <span class="tex-font-style-tt">ba</span> in $s$ as a <span class="tex-font-style-bf">substring</span>.</p><p>In one step, you can choose any index $i$ and replace $s_i$ with character <span class="tex-font-style-tt">a</span> or <span class="tex-font-style-tt">b</span>.</p><p>What is the minimum number of steps you need to make to achieve $\operatorname{AB}(s) = \operatorname{BA}(s)$?</p><p><span class="tex-font-style-bf">Reminder:</span></p><p>The number of occurrences of string $d$ in $s$ as substring is the number of indices $i$ ($1 \le i \le |s| - |d| + 1$) such that substring $s_i s_{i + 1} \dots s_{i + |d| - 1}$ is equal to $d$. For example, $\operatorname{AB}($<span class="tex-font-style-tt">aabbbabaa</span>$) = 2$ since there are two indices $i$: $i = 2$ where <span class="tex-font-style-tt">a<span class="tex-font-style-underline">ab</span>bbabaa</span> and $i = 6$ where <span class="tex-font-style-tt">aabbb<span class="tex-font-style-underline">ab</span>aa</span>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first and only line of each test case contains a single string $s$ ($1 \le |s| \le 100$, where $|s|$ is the length of the string $s$), consisting only of characters <span class="tex-font-style-tt">a</span> and/or <span class="tex-font-style-tt">b</span>.</p></div><div class="output-specification"><p>For each test case, print the resulting string $s$ with $\operatorname{AB}(s) = \operatorname{BA}(s)$ you'll get making the minimum number of steps.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first and only line of each test case contains a single string $s$ ($1 \le |s| \le 100$, where $|s|$ is the length of the string $s$), consisting only of characters <span class="tex-font-style-tt">a</span> and/or <span class="tex-font-style-tt">b</span>.</p>

## Output

<p>For each test case, print the resulting string $s$ with $\operatorname{AB}(s) = \operatorname{BA}(s)$ you'll get making the minimum number of steps.</p><p>If there are multiple answers, print any of them.</p>





```input1
4
b
aabbbabaa
abbb
abbaab
```




```output1
b
aabbbabaa
bbbb
abbaaa
```



## Note

<p>In the first test case, both $\operatorname{AB}(s) = 0$ and $\operatorname{BA}(s) = 0$ (there are no occurrences of <span class="tex-font-style-tt">ab</span> (<span class="tex-font-style-tt">ba</span>) in <span class="tex-font-style-tt">b</span>), so can leave $s$ untouched.</p><p>In the second test case, $\operatorname{AB}(s) = 2$ and $\operatorname{BA}(s) = 2$, so you can leave $s$ untouched. </p><p>In the third test case, $\operatorname{AB}(s) = 1$ and $\operatorname{BA}(s) = 0$. For example, we can change $s_1$ to <span class="tex-font-style-tt">b</span> and make both values zero.</p><p>In the fourth test case, $\operatorname{AB}(s) = 2$ and $\operatorname{BA}(s) = 1$. For example, we can change $s_6$ to <span class="tex-font-style-tt">a</span> and make both values equal to $1$.</p>
