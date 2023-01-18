## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is constraints</span>.</p><p>You are given a sequence $a$ consisting of $n$ positive integers.</p><p>Let's define a <span class="tex-font-style-bf">three blocks palindrome</span> as the sequence, consisting of <span class="tex-font-style-it">at most two</span> distinct elements (let these elements are $a$ and $b$, $a$ can be equal $b$) and is as follows: $[\underbrace{a, a, \dots, a}_{x}, \underbrace{b, b, \dots, b}_{y}, \underbrace{a, a, \dots, a}_{x}]$. There $x, y$ are integers greater than or equal to $0$. For example, sequences $[]$, $[2]$, $[1, 1]$, $[1, 2, 1]$, $[1, 2, 2, 1]$ and $[1, 1, 2, 1, 1]$ are <span class="tex-font-style-bf">three block palindromes</span> but $[1, 2, 3, 2, 1]$, $[1, 2, 1, 2, 1]$ and $[1, 2]$ are not.</p><p>Your task is to choose the maximum by length <span class="tex-font-style-bf">subsequence</span> of $a$ that is a <span class="tex-font-style-bf">three blocks palindrome</span>.</p><p>You have to answer $t$ independent test cases.</p><p>Recall that the sequence $t$ is a a subsequence of the sequence $s$ if $t$ can be derived from $s$ by removing zero or more elements without changing the order of the remaining elements. For example, if $s=[1, 2, 1, 3, 1, 2, 1]$, then possible subsequences are: $[1, 1, 1, 1]$, $[3]$ and $[1, 2, 1, 3, 1, 2, 1]$, but not $[3, 2, 3]$ and $[1, 1, 1, 1, 2]$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 200$), where $a_i$ is the $i$-th element of $a$. <span class="tex-font-style-bf">Note that the maximum value of $a_i$ can be up to $200$</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer — the maximum possible length of some subsequence of $a$ that is a <span class="tex-font-style-bf">three blocks palindrome</span>.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 200$), where $a_i$ is the $i$-th element of $a$. <span class="tex-font-style-bf">Note that the maximum value of $a_i$ can be up to $200$</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer — the maximum possible length of some subsequence of $a$ that is a <span class="tex-font-style-bf">three blocks palindrome</span>.</p>





```input1
6
8
1 1 2 2 3 2 1 1
3
1 3 3
4
1 10 10 1
1
26
2
2 1
3
1 1 1
```




```output1
7
2
4
1
1
3
```


