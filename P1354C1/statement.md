## Description

<div><p><span class="tex-font-style-bf">The statement of this problem is the same as the statement of problem C2. The only difference is that, in problem C1, $n$ is always even, and in C2, $n$ is always odd.</span></p><p>You are given a regular polygon with $2 \cdot n$ vertices (it's convex and has equal sides and equal angles) and all its sides have length $1$. Let's name it as $2n$-gon.</p><p>Your task is to find the square of the minimum size such that you can embed $2n$-gon in the square. Embedding $2n$-gon in the square means that you need to place $2n$-gon in the square in such way that each point which lies inside or on a border of $2n$-gon should also lie inside or on a border of the square.</p><p>You can rotate $2n$-gon and/or the square.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 200$)&nbsp;— the number of test cases.</p><p>Next $T$ lines contain descriptions of test cases&nbsp;— one per line. Each line contains single <span class="tex-font-style-bf">even</span> integer $n$ ($2 \le n \le 200$). Don't forget you need to embed $2n$-gon, not an $n$-gon.</p></div><div class="output-specification"><p>Print $T$ real numbers&nbsp;— one per test case. For each test case, print the minimum length of a side of the square $2n$-gon can be embedded in. Your answer will be considered correct if its absolute or relative error doesn't exceed $10^{-6}$.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 200$)&nbsp;— the number of test cases.</p><p>Next $T$ lines contain descriptions of test cases&nbsp;— one per line. Each line contains single <span class="tex-font-style-bf">even</span> integer $n$ ($2 \le n \le 200$). Don't forget you need to embed $2n$-gon, not an $n$-gon.</p>

## Output

<p>Print $T$ real numbers&nbsp;— one per test case. For each test case, print the minimum length of a side of the square $2n$-gon can be embedded in. Your answer will be considered correct if its absolute or relative error doesn't exceed $10^{-6}$.</p>





```input1
3
2
4
200
```




```output1
1.000000000
2.414213562
127.321336469
```


