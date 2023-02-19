## Description

<div><p>You are given two arrays $a$ and $b$ of $n$ elements, each element is either $0$ or $1$.</p><p>You can make operations of $2$ kinds. </p><ul> <li> Pick an index $i$ and change $a_i$ to $1-a_i$. </li><li> Rearrange the array $a$ however you want. </li></ul><p>Find the minimum number of operations required to make $a$ equal to $b$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 400$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$) — the length of the arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ space-separated integers $a_1,a_2,\ldots,a_n$ ($a_i$ is $0$ or $1$), representing the array $a$.</p><p>The third line of each test case contains $n$ space-separated integers $b_1,b_2,\ldots,b_n$ ($b_i$ is $0$ or $1$), representing the array $b$.</p></div><div class="output-specification"><p>For each test case, print the minimum number of operations required to make $a$ equal to $b$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 400$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$) — the length of the arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ space-separated integers $a_1,a_2,\ldots,a_n$ ($a_i$ is $0$ or $1$), representing the array $a$.</p><p>The third line of each test case contains $n$ space-separated integers $b_1,b_2,\ldots,b_n$ ($b_i$ is $0$ or $1$), representing the array $b$.</p>

## Output

<p>For each test case, print the minimum number of operations required to make $a$ equal to $b$.</p>





```input1|2,3,4,8,9,10,14,15,16
5
3
1 0 1
0 0 1
4
1 1 0 0
0 1 1 1
2
1 1
1 1
4
1 0 0 1
0 1 1 0
1
0
1
```




```output1
1
2
0
1
1
```



## Note

<p>In the first case, we need only one operation: change $a_1$ to $1-a_i$. Now $a = [0, 0]$ which is equal to $b$.</p><p>In the second case, the optimal way is to rearrange $a$ to get the array $[0, 1, 11$. Now $a = [0, 0, 1]$ which is equal to $b$.</p><p>In the second case, one of optimal ways would be to first change $a_3$ to $1 - a_3$, then rearrange $a$.</p><p>In the third case, no operation is needed.</p><p>In the fourth case, the optimal way is to rearrange $a$ to get the array $[0, 1, 1, 0]$.</p>
