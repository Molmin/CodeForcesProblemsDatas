## Description

<div><p>A positive integer $x$ is called a <span class="tex-font-style-it">power of two</span> if it can be represented as $x = 2^y$, where $y$ is a non-negative integer. So, the <span class="tex-font-style-it">powers of two</span> are $1, 2, 4, 8, 16, \dots$.</p><p>You are given two positive integers $n$ and $k$. Your task is to represent $n$ as the <span class="tex-font-style-bf">sum</span> of <span class="tex-font-style-bf">exactly</span> $k$ <span class="tex-font-style-it">powers of two</span>.</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $k$ ($1 \le n \le 10^9$, $1 \le k \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>If it is impossible to represent $n$ as the sum of $k$ powers of two, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span>, and then print $k$ positive integers $b_1, b_2, \dots, b_k$ such that each of $b_i$ is a power of two, and $\sum \limits_{i = 1}^{k} b_i = n$. If there are multiple answers, you may print any of them.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $k$ ($1 \le n \le 10^9$, $1 \le k \le 2 \cdot 10^5$).</p>

## Output

<p>If it is impossible to represent $n$ as the sum of $k$ powers of two, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span>, and then print $k$ positive integers $b_1, b_2, \dots, b_k$ such that each of $b_i$ is a power of two, and $\sum \limits_{i = 1}^{k} b_i = n$. If there are multiple answers, you may print any of them.</p>





```input1
9 4
```




```input2
8 1
```




```input3
5 1
```




```input4
3 7
```




```output1
YES
1 2 2 4
```




```output2
YES
8
```




```output3
NO
```




```output4
NO
```


