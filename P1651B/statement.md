## Description

<div><p>Recently, your friend discovered one special operation on an integer array $a$: </p><ol> <li> Choose two indices $i$ and $j$ ($i \neq j$); </li><li> Set $a_i = a_j = |a_i - a_j|$. </li></ol><p>After playing with this operation for a while, he came to the next conclusion: </p><ul> <li> For every array $a$ of $n$ integers, where $1 \le a_i \le 10^9$, you can find a pair of indices $(i, j)$ such that the total sum of $a$ will <span class="tex-font-style-bf">decrease</span> after performing the operation. </li></ul><p>This statement sounds fishy to you, so you want to find a counterexample for a given integer $n$. Can you find such counterexample and prove him wrong?</p><p>In other words, find an array $a$ consisting of $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) such that for all pairs of indices $(i, j)$ performing the operation won't decrease the total sum (it will increase or not change the sum).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first and only line of each test case contains a single integer $n$ ($2 \le n \le 1000$)&nbsp;— the length of array $a$.</p></div><div class="output-specification"><p>For each test case, if there is no counterexample array $a$ of size $n$, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span> followed by the array $a$ itself ($1 \le a_i \le 10^9$). If there are multiple counterexamples, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first and only line of each test case contains a single integer $n$ ($2 \le n \le 1000$)&nbsp;— the length of array $a$.</p>

## Output

<p>For each test case, if there is no counterexample array $a$ of size $n$, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span> followed by the array $a$ itself ($1 \le a_i \le 10^9$). If there are multiple counterexamples, print any.</p>





```input1
3
2
512
3
```




```output1
YES
1 337
NO
YES
31 4 159
```



## Note

<p>In the first test case, the only possible pairs of indices are $(1, 2)$ and $(2, 1)$.</p><p>If you perform the operation on indices $(1, 2)$ (or $(2, 1)$), you'll get $a_1 = a_2 = |1 - 337| = 336$, or array $[336, 336]$. In both cases, the total sum increases, so this array $a$ is a counterexample.</p>
