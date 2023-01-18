## Description

<div><p>Vasya likes to solve equations. Today he wants to solve $(x~\mathrm{div}~k) \cdot (x \bmod k) = n$, where $\mathrm{div}$ and $\mathrm{mod}$ stand for integer division and modulo operations (refer to the Notes below for exact definition). In this equation, $k$ and $n$ are positive integer parameters, and $x$ is a positive integer unknown. If there are several solutions, Vasya wants to find the smallest possible $x$. Can you help him?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 10^6$, $2 \leq k \leq 1000$).</p></div><div class="output-specification"><p>Print a single integer $x$&nbsp;— the smallest positive integer solution to $(x~\mathrm{div}~k) \cdot (x \bmod k) = n$. It is guaranteed that this equation has at least one positive integer solution.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 10^6$, $2 \leq k \leq 1000$).</p>

## Output

<p>Print a single integer $x$&nbsp;— the smallest positive integer solution to $(x~\mathrm{div}~k) \cdot (x \bmod k) = n$. It is guaranteed that this equation has at least one positive integer solution.</p>





```input1
6 3
```




```input2
1 2
```




```input3
4 6
```




```output1
11
```




```output2
3
```




```output3
10
```



## Note

<p>The result of integer division $a~\mathrm{div}~b$ is equal to the largest integer $c$ such that $b \cdot c \leq a$. $a$ modulo $b$ (shortened $a \bmod b$) is the only integer $c$ such that $0 \leq c &lt; b$, and $a - c$ is divisible by $b$.</p><p>In the first sample, $11~\mathrm{div}~3 = 3$ and $11 \bmod 3 = 2$. Since $3 \cdot 2 = 6$, then $x = 11$ is a solution to $(x~\mathrm{div}~3) \cdot (x \bmod 3) = 6$. One can see that $19$ is the only other positive integer solution, hence $11$ is the smallest one.</p>
