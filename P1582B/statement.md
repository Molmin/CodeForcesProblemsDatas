## Description

<div><p>Luntik came out for a morning stroll and found an array $a$ of length $n$. He calculated the sum $s$ of the elements of the array ($s= \sum_{i=1}^{n} a_i$). Luntik calls a subsequence of the array $a$ <span class="tex-font-style-it">nearly full</span> if the sum of the numbers in that subsequence is equal to $s-1$.</p><p>Luntik really wants to know the number of <span class="tex-font-style-it">nearly full</span> subsequences of the array $a$. But he needs to come home so he asks you to solve that problem!</p><p>A sequence $x$ is a subsequence of a sequence $y$ if $x$ can be obtained from $y$ by deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. The next $2 \cdot t$ lines contain descriptions of test cases. The description of each test case consists of two lines.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 60$) — the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) — the elements of the array $a$.</p></div><div class="output-specification"><p>For each test case print the number of <span class="tex-font-style-it">nearly full</span> subsequences of the array.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. The next $2 \cdot t$ lines contain descriptions of test cases. The description of each test case consists of two lines.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 60$) — the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) — the elements of the array $a$.</p>

## Output

<p>For each test case print the number of <span class="tex-font-style-it">nearly full</span> subsequences of the array.</p>





```input1
5
5
1 2 3 4 5
2
1000 1000
2
1 0
5
3 0 2 1 1
5
2 1 0 3 0
```




```output1
1
0
2
4
4
```



## Note

<p>In the first test case, $s=1+2+3+4+5=15$, only $(2,3,4,5)$ is a nearly full subsequence among all subsequences, the sum in it is equal to $2+3+4+5=14=15-1$.</p><p>In the second test case, there are no nearly full subsequences.</p><p>In the third test case, $s=1+0=1$, the nearly full subsequences are $(0)$ and $()$ (the sum of an empty subsequence is $0$).</p>
