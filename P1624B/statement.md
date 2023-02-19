## Description

<div><p>Polycarp has $3$ positive integers $a$, $b$ and $c$. He can perform the following operation <span class="tex-font-style-bf">exactly once</span>.</p><ul> <li> Choose a <span class="tex-font-style-bf">positive</span> integer $m$ and multiply <span class="tex-font-style-bf">exactly one</span> of the integers $a$, $b$ or $c$ by $m$. </li></ul><p>Can Polycarp make it so that after performing the operation, the sequence of three numbers $a$, $b$, $c$ (<span class="tex-font-style-bf">in this order</span>) forms an <a href="https://en.wikipedia.org/wiki/Arithmetic_progression">arithmetic progression</a>? Note that you <span class="tex-font-style-bf">cannot change</span> the order of $a$, $b$ and $c$.</p><p>Formally, a sequence $x_1, x_2, \dots, x_n$ is called an arithmetic progression (AP) if there exists a number $d$ (called "common difference") such that $x_{i+1}=x_i+d$ for all $i$ from $1$ to $n-1$. In this problem, $n=3$.</p><p>For example, the following sequences are AP: $[5, 10, 15]$, $[3, 2, 1]$, $[1, 1, 1]$, and $[13, 10, 7]$. The following sequences are not AP: $[1, 2, 4]$, $[0, 1, 0]$ and $[1, 3, 2]$.</p><p>You need to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line contains the number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each of the following $t$ lines contains $3$ integers $a$, $b$, $c$ ($1 \le a, b, c \le 10^8$).</p></div><div class="output-specification"><p>For each test case print <span class="tex-font-style-tt">"YES"</span> (without quotes) if Polycarp can choose a <span class="tex-font-style-bf">positive</span> integer $m$ and multiply <span class="tex-font-style-bf">exactly one</span> of the integers $a$, $b$ or $c$ by $m$ to make $[a, b, c]$ be an arithmetic progression. Print <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p><p>You can print <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any (upper or lower) case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains the number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each of the following $t$ lines contains $3$ integers $a$, $b$, $c$ ($1 \le a, b, c \le 10^8$).</p>

## Output

<p>For each test case print <span class="tex-font-style-tt">"YES"</span> (without quotes) if Polycarp can choose a <span class="tex-font-style-bf">positive</span> integer $m$ and multiply <span class="tex-font-style-bf">exactly one</span> of the integers $a$, $b$ or $c$ by $m$ to make $[a, b, c]$ be an arithmetic progression. Print <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p><p>You can print <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any (upper or lower) case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p>





```input1
11
10 5 30
30 5 10
1 2 3
1 6 3
2 6 3
1 1 1
1 1 2
1 1 3
1 100000000 1
2 1 1
1 2 2
```




```output1
YES
YES
YES
YES
NO
YES
NO
YES
YES
NO
YES
```



## Note

<p>In the first and second test cases, you can choose the number $m=4$ and multiply the second number ($b=5$) by $4$.</p><p>In the first test case the resulting sequence will be $[10, 20, 30]$. This is an AP with a difference $d=10$.</p><p>In the second test case the resulting sequence will be $[30, 20, 10]$. This is an AP with a difference $d=-10$.</p><p>In the third test case, you can choose $m=1$ and multiply any number by $1$. The resulting sequence will be $[1, 2, 3]$. This is an AP with a difference $d=1$.</p><p>In the fourth test case, you can choose $m=9$ and multiply the first number ($a=1$) by $9$. The resulting sequence will be $[9, 6, 3]$. This is an AP with a difference $d=-3$.</p><p>In the fifth test case, it is impossible to make an AP.</p>
