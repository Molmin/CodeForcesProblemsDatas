## Description

<div><p>You are given the array $a$ consisting of $n$ positive (greater than zero) integers.</p><p>In one move, you can choose two indices $i$ and $j$ ($i \ne j$) such that the absolute difference between $a_i$ and $a_j$ is no more than one ($|a_i - a_j| \le 1$) and remove the smallest of these two elements. If two elements are equal, you can remove any of them (but exactly one).</p><p>Your task is to find if it is possible to obtain the array consisting of <span class="tex-font-style-bf">only one element</span> using several (possibly, zero) such moves or not.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 50$) — the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>For each test case, print the answer: "<span class="tex-font-style-tt">YES</span>" if it is possible to obtain the array consisting of <span class="tex-font-style-bf">only one element</span> using several (possibly, zero) moves described in the problem statement, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 50$) — the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>For each test case, print the answer: "<span class="tex-font-style-tt">YES</span>" if it is possible to obtain the array consisting of <span class="tex-font-style-bf">only one element</span> using several (possibly, zero) moves described in the problem statement, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
5
3
1 2 2
4
5 5 5 5
3
1 2 4
4
1 3 4 4
1
100
```




```output1
YES
YES
NO
NO
YES
```



## Note

<p>In the first test case of the example, we can perform the following sequence of moves:</p><ul> <li> choose $i=1$ and $j=3$ and remove $a_i$ (so $a$ becomes $[2; 2]$); </li><li> choose $i=1$ and $j=2$ and remove $a_j$ (so $a$ becomes $[2]$). </li></ul><p>In the second test case of the example, we can choose any possible $i$ and $j$ any move and it doesn't matter which element we remove.</p><p>In the third test case of the example, there is no way to get rid of $2$ and $4$.</p>
