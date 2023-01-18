## Description

<div><p>Integer factorisation is hard. The RSA Factoring Challenge offered $$100\,000$ for factoring RSA-$1024$, a $1024$-bit long product of two prime numbers. To this date, nobody was able to claim the prize. We want you to factorise a $1024$-bit number.</p><p>Since your programming language of choice might not offer facilities for handling large integers, we will provide you with a very simple calculator. </p><p>To use this calculator, you can print queries on the standard output and retrieve the results from the standard input. The operations are as follows: </p><ul> <li> <span class="tex-font-style-tt">+ x y</span> where $x$ and $y$ are integers between $0$ and $n-1$. Returns $(x+y) \bmod n$. </li><li> <span class="tex-font-style-tt">- x y</span> where $x$ and $y$ are integers between $0$ and $n-1$. Returns $(x-y) \bmod n$. </li><li> <span class="tex-font-style-tt">* x y</span> where $x$ and $y$ are integers between $0$ and $n-1$. Returns $(x \cdot y) \bmod n$. </li><li> <span class="tex-font-style-tt">/ x y</span> where $x$ and $y$ are integers between $0$ and $n-1$ and $y$ is coprime with $n$. Returns $(x \cdot y^{-1}) \bmod n$ where $y^{-1}$ is multiplicative inverse of $y$ modulo $n$. If $y$ is not coprime with $n$, then $-1$ is returned instead. </li><li> <span class="tex-font-style-tt">sqrt x</span> where $x$ is integer between $0$ and $n-1$ coprime with $n$. Returns $y$ such that $y^2 \bmod n = x$. If there are multiple such integers, only one of them is returned. If there are none, $-1$ is returned instead. </li><li> <span class="tex-font-style-tt">^ x y</span> where $x$ and $y$ are integers between $0$ and $n-1$. Returns ${x^y \bmod n}$. </li></ul><p>Find the factorisation of $n$ that is a product of between $2$ and $10$ <span class="tex-font-style-bf">distinct</span> prime numbers, all of form $4x + 3$ for some integer $x$.</p><p><span class="tex-font-style-bf">Because of technical issues, we restrict number of requests to $100$.</span></p></div><div class="input-specification"><p>The only line contains a single integer $n$&nbsp;($21 \leq n \leq 2^{1024}$). It is guaranteed that $n$ is a product of between $2$ and $10$ distinct prime numbers, all of form $4x + 3$ for some integer $x$.</p></div><div class="output-specification"><p>You can print as many queries as you wish, adhering to the time limit (see the Interaction section for more details). </p><p>When you think you know the answer, output a single line of form <span class="tex-font-style-tt">! k p_1 p_2 ... p_k</span>, where $k$ is the number of prime factors of $n$, and $p_i$ are the distinct prime factors. You may print the factors in any order.</p><p><span class="tex-font-style-bf">Hacks input</span></p><p>For hacks, use the following format:. </p><p>The first should contain $k$ ($2 \leq k \leq 10$)&nbsp;— the number of prime factors of $n$. </p><p>The second should contain $k$ space separated integers $p_1, p_2, \dots, p_k$ ($21 \leq n \leq 2^{1024}$)&nbsp;— the prime factors of $n$. All prime factors have to be of form $4x + 3$ for some integer $x$. They all have to be distinct. </p></div><div><h2>Interaction</h2><p>After printing a query do not forget to output end of line and flush the output. Otherwise you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>The number of queries is not limited. However, your program must (as always) fit in the time limit. The run time of the interactor is also counted towards the time limit. The maximum runtime of each query is given below.</p><ul> <li> <span class="tex-font-style-tt">+ x y</span>&nbsp;— up to $1$ ms. </li><li> <span class="tex-font-style-tt">- x y</span>&nbsp;— up to $1$ ms. </li><li> <span class="tex-font-style-tt">* x y</span>&nbsp;— up to $1$ ms. </li><li> <span class="tex-font-style-tt">/ x y</span>&nbsp;— up to $350$ ms. </li><li> <span class="tex-font-style-tt">sqrt x</span>&nbsp;— up to $80$ ms. </li><li> <span class="tex-font-style-tt">^ x y</span>&nbsp;— up to $350$ ms. </li></ul><p>Note that the sample input contains extra empty lines so that it easier to read. The real input will not contain any empty lines and you do not need to output extra empty lines.</p></div>

## Input

<p>The only line contains a single integer $n$&nbsp;($21 \leq n \leq 2^{1024}$). It is guaranteed that $n$ is a product of between $2$ and $10$ distinct prime numbers, all of form $4x + 3$ for some integer $x$.</p>

## Output

<p>You can print as many queries as you wish, adhering to the time limit (see the Interaction section for more details). </p><p>When you think you know the answer, output a single line of form <span class="tex-font-style-tt">! k p_1 p_2 ... p_k</span>, where $k$ is the number of prime factors of $n$, and $p_i$ are the distinct prime factors. You may print the factors in any order.</p><p><span class="tex-font-style-bf">Hacks input</span></p><p>For hacks, use the following format:. </p><p>The first should contain $k$ ($2 \leq k \leq 10$)&nbsp;— the number of prime factors of $n$. </p><p>The second should contain $k$ space separated integers $p_1, p_2, \dots, p_k$ ($21 \leq n \leq 2^{1024}$)&nbsp;— the prime factors of $n$. All prime factors have to be of form $4x + 3$ for some integer $x$. They all have to be distinct. </p>





```input1
21

7

17

15

17

11

-1

15


```




```output1
+ 12 16

- 6 10

* 8 15

/ 5 4

sqrt 16

sqrt 5

^ 6 12

! 2 3 7
```



## Note

<p>We start by reading the first line containing the integer $n = 21$. Then, we ask for: </p><ol> <li> $(12 + 16) \bmod 21 = 28 \bmod 21 = 7$. </li><li> $(6 - 10) \bmod 21 = -4 \bmod 21 = 17$. </li><li> $(8 \cdot 15) \bmod 21 = 120 \bmod 21 = 15$. </li><li> $(5 \cdot 4^{-1}) \bmod 21 = (5 \cdot 16) \bmod 21 = 80 \bmod 21 = 17$. </li><li> Square root of $16$. The answer is $11$, as $(11 \cdot 11) \bmod 21 = 121 \bmod 21 = 16$. Note that the answer may as well be $10$. </li><li> Square root of $5$. There is no $x$ such that $x^2 \bmod 21 = 5$, so the output is $-1$. </li><li> $(6^{12}) \bmod 21 = 2176782336 \bmod 21 = 15$. </li></ol><p>We conclude that our calculator is working, stop fooling around and realise that $21 = 3 \cdot 7$.</p>
