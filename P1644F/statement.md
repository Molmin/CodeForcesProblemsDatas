## Description

<div><p>For an array of integers $a$, let's define $|a|$ as the number of elements in it.</p><p>Let's denote two functions:</p><ul><li> $F(a, k)$ is a function that takes an array of integers $a$ and a positive integer $k$. The result of this function is the array containing $|a|$ first elements of the array that you get by replacing each element of $a$ with exactly $k$ copies of that element.<p>For example, $F([2, 2, 1, 3, 5, 6, 8], 2)$ is calculated as follows: first, you replace each element of the array with $2$ copies of it, so you obtain $[2, 2, 2, 2, 1, 1, 3, 3, 5, 5, 6, 6, 8, 8]$. Then, you take the first $7$ elements of the array you obtained, so the result of the function is $[2, 2, 2, 2, 1, 1, 3]$.</p></li><li> $G(a, x, y)$ is a function that takes an array of integers $a$ and two <span class="tex-font-style-bf">different</span> integers $x$ and $y$. The result of this function is the array $a$ with every element equal to $x$ replaced by $y$, and every element equal to $y$ replaced by $x$.<p>For example, $G([1, 1, 2, 3, 5], 3, 1) = [3, 3, 2, 1, 5]$.</p></li></ul><p>An array $a$ is a <span class="tex-font-style-bf">parent</span> of the array $b$ if:</p><ul> <li> either there exists a positive integer $k$ such that $F(a, k) = b$; </li><li> or there exist two different integers $x$ and $y$ such that $G(a, x, y) = b$. </li></ul><p>An array $a$ is an <span class="tex-font-style-bf">ancestor</span> of the array $b$ if there exists a finite sequence of arrays $c_0, c_1, \dots, c_m$ ($m \ge 0$) such that $c_0$ is $a$, $c_m$ is $b$, and for every $i \in [1, m]$, $c_{i-1}$ is a parent of $c_i$.</p><p><span class="tex-font-style-it">And now, the problem itself</span>.</p><p>You are given two integers $n$ and $k$. Your goal is to construct a sequence of arrays $s_1, s_2, \dots, s_m$ in such a way that:</p><ul> <li> every array $s_i$ contains exactly $n$ elements, and all elements are integers from $1$ to $k$; </li><li> for every array $a$ consisting of exactly $n$ integers from $1$ to $k$, the sequence contains at least one array $s_i$ such that $s_i$ is an ancestor of $a$. </li></ul><p>Print the minimum number of arrays in such sequence.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $k$ ($1 \le n, k \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Print one integer — the minimum number of elements in a sequence of arrays meeting the constraints. Since the answer can be large, output it modulo $998244353$.</p></div>

## Input

<p>The only line contains two integers $n$ and $k$ ($1 \le n, k \le 2 \cdot 10^5$).</p>

## Output

<p>Print one integer — the minimum number of elements in a sequence of arrays meeting the constraints. Since the answer can be large, output it modulo $998244353$.</p>





```input1
3 2
```




```input2
4 10
```




```input3
13 37
```




```input4
1337 42
```




```input5
198756 123456
```




```input6
123456 198756
```




```output1
2
```




```output2
12
```




```output3
27643508
```




```output4
211887828
```




```output5
159489391
```




```output6
460526614
```



## Note

<p>Let's analyze the first example.</p><p>One of the possible answers for the first example is the sequence $[[2, 1, 2], [1, 2, 2]]$. Every array of size $3$ consisting of elements from $1$ to $2$ has an ancestor in this sequence:</p><ul> <li> for the array $[1, 1, 1]$, the ancestor is $[1, 2, 2]$: $F([1, 2, 2], 13) = [1, 1, 1]$; </li><li> for the array $[1, 1, 2]$, the ancestor is $[1, 2, 2]$: $F([1, 2, 2], 2) = [1, 1, 2]$; </li><li> for the array $[1, 2, 1]$, the ancestor is $[2, 1, 2]$: $G([2, 1, 2], 1, 2) = [1, 2, 1]$; </li><li> for the array $[1, 2, 2]$, the ancestor is $[1, 2, 2]$; </li><li> for the array $[2, 1, 1]$, the ancestor is $[1, 2, 2]$: $G([1, 2, 2], 1, 2) = [2, 1, 1]$; </li><li> for the array $[2, 1, 2]$, the ancestor is $[2, 1, 2]$; </li><li> for the array $[2, 2, 1]$, the ancestor is $[2, 1, 2]$: $F([2, 1, 2], 2) = [2, 2, 1]$; </li><li> for the array $[2, 2, 2]$, the ancestor is $[1, 2, 2]$: $G(F([1, 2, 2], 4), 1, 2) = G([1, 1, 1], 1, 2) = [2, 2, 2]$. </li></ul>
