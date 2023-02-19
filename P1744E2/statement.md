## Description

<div><p><span class="tex-font-style-bf">This is an hard version of the problem. The only difference between an easy and a hard version is the constraints on $a$, $b$, $c$ and $d$.</span></p><p>You are given $4$ positive integers $a$, $b$, $c$, $d$ with $a &lt; c$ and $b &lt; d$. Find any pair of numbers $x$ and $y$ that satisfies the following conditions:</p><ul><li> $a &lt; x \leq c$, $b &lt; y \leq d$,</li><li> $x \cdot y$ is divisible by $a \cdot b$.</li></ul><p>Note that required $x$ and $y$ may not exist.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10$), the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The only line of each test case contains four integers $a$, $b$, $c$ and $d$ ($1 \leq a &lt; c \leq 10^9$, $1 \leq b &lt; d \leq 10^9$).</p></div><div class="output-specification"><p>For each test case print a pair of numbers $a &lt; x \leq c$ and $b &lt; y \leq d$ such that $x \cdot y$ is divisible by $a \cdot b$. If there are multiple answers, print any of them. If there is no such pair of numbers, then print <span class="tex-font-style-tt">-1 -1</span>.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10$), the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The only line of each test case contains four integers $a$, $b$, $c$ and $d$ ($1 \leq a &lt; c \leq 10^9$, $1 \leq b &lt; d \leq 10^9$).</p>

## Output

<p>For each test case print a pair of numbers $a &lt; x \leq c$ and $b &lt; y \leq d$ such that $x \cdot y$ is divisible by $a \cdot b$. If there are multiple answers, print any of them. If there is no such pair of numbers, then print <span class="tex-font-style-tt">-1 -1</span>.</p>





```input1|2,4,6,8,10
10
1 1 2 2
3 4 5 7
8 9 15 18
12 21 14 24
36 60 48 66
1024 729 373248 730
1024 729 373247 730
5040 40320 40319 1000000000
999999999 999999999 1000000000 1000000000
268435456 268435456 1000000000 1000000000
```




```output1
2 2
4 6
12 12
-1 -1
-1 -1
373248 730
-1 -1
15120 53760
-1 -1
536870912 536870912
```


