## Description

<div><p>You are given two arrays $a$ and $b$, both of length $n$. All elements of both arrays are from $0$ to $n-1$.</p><p>You can reorder elements of the array $b$ (if you want, you may leave the order of elements as it is). After that, let array $c$ be the array of length $n$, the $i$-th element of this array is $c_i = (a_i + b_i) \% n$, where $x \% y$ is $x$ modulo $y$.</p><p>Your task is to reorder elements of the array $b$ to obtain the <span class="tex-font-style-bf">lexicographically</span> minimum possible array $c$.</p><p>Array $x$ of length $n$ is lexicographically less than array $y$ of length $n$, if there exists such $i$ ($1 \le i \le n$), that $x_i &lt; y_i$, and for any $j$ ($1 \le j &lt; i$) $x_j = y_j$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$, $b$ and $c$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; n$), where $a_i$ is the $i$-th element of $a$.</p><p>The third line of the input contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i &lt; n$), where $b_i$ is the $i$-th element of $b$.</p></div><div class="output-specification"><p>Print the <span class="tex-font-style-bf">lexicographically</span> minimum possible array $c$. Recall that your task is to reorder elements of the array $b$ and obtain the <span class="tex-font-style-bf">lexicographically</span> minimum possible array $c$, where the $i$-th element of $c$ is $c_i = (a_i + b_i) \% n$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$, $b$ and $c$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; n$), where $a_i$ is the $i$-th element of $a$.</p><p>The third line of the input contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i &lt; n$), where $b_i$ is the $i$-th element of $b$.</p>

## Output

<p>Print the <span class="tex-font-style-bf">lexicographically</span> minimum possible array $c$. Recall that your task is to reorder elements of the array $b$ and obtain the <span class="tex-font-style-bf">lexicographically</span> minimum possible array $c$, where the $i$-th element of $c$ is $c_i = (a_i + b_i) \% n$.</p>





```input1
4
0 1 2 1
3 2 1 1
```




```input2
7
2 5 1 5 3 4 3
2 4 3 5 6 5 1
```




```output1
1 0 0 2
```




```output2
0 0 0 1 0 2 4
```


