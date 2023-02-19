## Description

<div><div class="epigraph"><div class="epigraph-text">Ran is especially skilled in computation and mathematics. It is said that she can do unimaginable calculation work in an instant.</div><div class="epigraph-source">—<span class="tex-font-style-it">Perfect Memento in Strict Sense</span></div></div><p>Ran Yakumo is a cute girl who loves creating cute Maths problems.</p><p>Let $f(x)$ be the minimal <a href="https://en.wikipedia.org/wiki/Square_number">square number</a> <span class="tex-font-style-bf">strictly</span> greater than $x$, and $g(x)$ be the maximal square number less than or equal to $x$. For example, $f(1)=f(2)=g(4)=g(8)=4$.</p><p>A positive integer $x$ is <span class="tex-font-style-it">cute</span> if $x-g(x)&lt;f(x)-x$. For example, $1,5,11$ are cute integers, while $3,8,15$ are not. </p><p>Ran gives you an array $a$ of length $n$. She wants you to find the smallest non-negative integer $k$ such that $a_i + k$ is a cute number for any element of $a$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^6$) — the length of $a$.</p><p>The second line contains $n$ intergers $a_1,a_2,\ldots,a_n$ ($1 \leq a_1 \leq a_2 \leq \ldots \leq a_n \leq 2\cdot 10^6$) — the array $a$.</p></div><div class="output-specification"><p>Print a single interger $k$ — the answer.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^6$) — the length of $a$.</p><p>The second line contains $n$ intergers $a_1,a_2,\ldots,a_n$ ($1 \leq a_1 \leq a_2 \leq \ldots \leq a_n \leq 2\cdot 10^6$) — the array $a$.</p>

## Output

<p>Print a single interger $k$ — the answer.</p>





```input1
4
1 3 8 10
```




```input2
5
2 3 8 9 11
```




```input3
8
1 2 3 4 5 6 7 8
```




```output1
1
```




```output2
8
```




```output3
48
```



## Note

<p>Test case 1:</p><p>$3$ is not cute integer, so $k\ne 0$.</p><p>$2,4,9,11$ are cute integers, so $k=1$.</p>
