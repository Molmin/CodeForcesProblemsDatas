## Description

<div><p>The length of the <span class="tex-font-style-bf">longest common prefix</span> of two strings $s = s_1 s_2 \ldots s_n$ and $t = t_1 t_2 \ldots t_m$ is defined as the maximum integer $k$ ($0 \le k \le min(n,m)$) such that $s_1 s_2 \ldots s_k$ equals $t_1 t_2 \ldots t_k$.</p><p>Koa the Koala initially has $n+1$ strings $s_1, s_2, \dots, s_{n+1}$.</p><p>For each $i$ ($1 \le i \le n$) she calculated $a_i$&nbsp;— the length of the <span class="tex-font-style-bf">longest common prefix</span> of $s_i$ and $s_{i+1}$.</p><p>Several days later Koa found these numbers, but she couldn't remember the strings.</p><p>So Koa would like to find some strings $s_1, s_2, \dots, s_{n+1}$ which would have generated numbers $a_1, a_2, \dots, a_n$. Can you help her?</p><p>If there are many answers print any. We can show that answer always exists for the given constraints. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of elements in the list $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 50$)&nbsp;— the elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p></div><div class="output-specification"><p>For each test case:</p><p>Output $n+1$ lines. In the $i$-th line print string $s_i$ ($1 \le |s_i| \le 200$), <span class="tex-font-style-bf">consisting of lowercase Latin letters</span>. Length of the longest common prefix of strings $s_i$ and $s_{i+1}$ has to be equal to $a_i$.</p><p>If there are many answers print any. We can show that answer always exists for the given constraints.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of elements in the list $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 50$)&nbsp;— the elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p>

## Output

<p>For each test case:</p><p>Output $n+1$ lines. In the $i$-th line print string $s_i$ ($1 \le |s_i| \le 200$), <span class="tex-font-style-bf">consisting of lowercase Latin letters</span>. Length of the longest common prefix of strings $s_i$ and $s_{i+1}$ has to be equal to $a_i$.</p><p>If there are many answers print any. We can show that answer always exists for the given constraints.</p>





```input1
4
4
1 2 4 2
2
5 3
3
1 3 1
3
0 0 0
```




```output1
aeren
ari
arousal
around
ari
monogon
monogamy
monthly
kevinvu
kuroni
kurioni
korone
anton
loves
adhoc
problems
```



## Note

<p>In the $1$-st test case one of the possible answers is $s = [aeren, ari, arousal, around, ari]$.</p><p>Lengths of longest common prefixes are:</p><ul> <li> Between $\color{red}{a}eren$ and $\color{red}{a}ri$ $\rightarrow 1$ </li><li> Between $\color{red}{ar}i$ and $\color{red}{ar}ousal$ $\rightarrow 2$ </li><li> Between $\color{red}{arou}sal$ and $\color{red}{arou}nd$ $\rightarrow 4$ </li><li> Between $\color{red}{ar}ound$ and $\color{red}{ar}i$ $\rightarrow 2$ </li></ul>
