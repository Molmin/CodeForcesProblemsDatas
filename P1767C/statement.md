## Description

<div><p>You are given an integer $n$. You have to calculate the number of binary (consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>) strings $s$ meeting the following constraints.</p><p>For every pair of integers $(i, j)$ such that $1 \le i \le j \le n$, an integer $a_{i,j}$ is given. It imposes the following constraint on the string $s_i s_{i+1} s_{i+2} \dots s_j$:</p><ul> <li> if $a_{i,j} = 1$, all characters in $s_i s_{i+1} s_{i+2} \dots s_j$ should be the same; </li><li> if $a_{i,j} = 2$, there should be at least two different characters in $s_i s_{i+1} s_{i+2} \dots s_j$; </li><li> if $a_{i,j} = 0$, there are no additional constraints on the string $s_i s_{i+1} s_{i+2} \dots s_j$. </li></ul><p>Count the number of binary strings $s$ of length $n$ meeting the aforementioned constraints. Since the answer can be large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 100$).</p><p>Then $n$ lines follow. The $i$-th of them contains $n-i+1$ integers $a_{i,i}, a_{i,i+1}, a_{i,i+2}, \dots, a_{i,n}$ ($0 \le a_{i,j} \le 2$).</p></div><div class="output-specification"><p>Print one integer — the number of strings meeting the constraints, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 100$).</p><p>Then $n$ lines follow. The $i$-th of them contains $n-i+1$ integers $a_{i,i}, a_{i,i+1}, a_{i,i+2}, \dots, a_{i,n}$ ($0 \le a_{i,j} \le 2$).</p>

## Output

<p>Print one integer — the number of strings meeting the constraints, taken modulo $998244353$.</p>





```input1
3
1 0 2
1 0
1
```




```input2
3
1 1 2
1 0
1
```




```input3
3
1 2 1
1 0
1
```




```input4
3
2 0 2
0 1
1
```




```output1
6
```




```output2
2
```




```output3
0
```




```output4
0
```



## Note

<p>In the first example, the strings meeting the constraints are <span class="tex-font-style-tt">001</span>, <span class="tex-font-style-tt">010</span>, <span class="tex-font-style-tt">011</span>, <span class="tex-font-style-tt">100</span>, <span class="tex-font-style-tt">101</span>, <span class="tex-font-style-tt">110</span>.</p><p>In the second example, the strings meeting the constraints are <span class="tex-font-style-tt">001</span>, <span class="tex-font-style-tt">110</span>.</p>
