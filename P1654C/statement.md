## Description

<div><p>Alice has a cake, and she is going to cut it. She will perform the following operation $n-1$ times: choose a piece of the cake (initially, the cake is all one piece) with weight $w\ge 2$ and cut it into two smaller pieces of weight $\lfloor\frac{w}{2}\rfloor$ and $\lceil\frac{w}{2}\rceil$ ($\lfloor x \rfloor$ and $\lceil x \rceil$ denote <a href="https://en.wikipedia.org/wiki/Floor_and_ceiling_functions">floor and ceiling functions</a>, respectively).</p><p>After cutting the cake in $n$ pieces, she will line up these $n$ pieces on a table in an arbitrary order. Let $a_i$ be the weight of the $i$-th piece in the line.</p><p>You are given the array $a$. Determine whether there exists an initial weight and sequence of operations which results in $a$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line: print <span class="tex-font-style-tt">YES</span> if the array $a$ could have resulted from Alice's operations, otherwise print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line: print <span class="tex-font-style-tt">YES</span> if the array $a$ could have resulted from Alice's operations, otherwise print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p>





```input1
14
1
327
2
869 541
2
985214736 985214737
3
2 3 1
3
2 3 3
6
1 1 1 1 1 1
6
100 100 100 100 100 100
8
100 100 100 100 100 100 100 100
8
2 16 1 8 64 1 4 32
10
1 2 4 7 1 1 1 1 7 2
10
7 1 1 1 3 1 3 3 2 3
10
1 4 4 1 1 1 3 3 3 1
10
2 3 2 2 1 2 2 2 2 2
4
999999999 999999999 999999999 999999999
```




```output1
YES
NO
YES
YES
NO
YES
NO
YES
YES
YES
YES
NO
NO
YES
```



## Note

<p>In the first test case, it's possible to get the array $a$ by performing $0$ operations on a cake with weight $327$.</p><p>In the second test case, it's not possible to get the array $a$.</p><p>In the third test case, it's possible to get the array $a$ by performing $1$ operation on a cake with weight $1\,970\,429\,473$: </p><ul> <li> Cut it in half, so that the weights are $[985\,214\,736, 985\,214\,737]$. </li></ul> Note that the starting weight can be greater than $10^9$.<p>In the fourth test case, it's possible to get the array $a$ by performing $2$ operations on a cake with weight $6$:</p><ul> <li> Cut it in half, so that the weights are $[3,3]$. </li><li> Cut one of the two pieces with weight $3$, so that the new weights are $[1, 2, 3]$ which is equivalent to $[2, 3, 1]$ up to reordering.</li></ul>
