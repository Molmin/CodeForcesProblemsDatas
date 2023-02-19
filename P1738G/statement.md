## Description

<div><p>You are given an $n \times n$ grid. </p><p>We write $(i, j)$ to denote the cell in the $i$-th row and $j$-th column. For each cell, you are told whether yon can delete it or not. </p><p>Given an integer $k$, you are asked to delete <span class="tex-font-style-bf">exactly</span> $(n-k+1)^2$ cells from the grid such that the following condition holds. </p><ul> <li> You cannot find $k$ not deleted cells $(x_1, y_1), (x_2, y_2), \dots, (x_k, y_k)$ that are strictly increasing, i.e., $x_i &lt; x_{i+1}$ and $y_i &lt; y_{i+1}$ for all $1 \leq i &lt; k$. </li></ul> Your task is to find a solution, or report that it is impossible. </div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \leq k \leq n \leq 1000$). </p><p>Then $n$ lines follow. The $i$-th line contains a binary string $s_i$ of length $n$. The $j$-th character of $s_i$ is <span class="tex-font-style-tt">1</span> if you can delete cell $(i, j)$, and <span class="tex-font-style-tt">0</span> otherwise.</p><p>It's guaranteed that the sum of $n^2$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, if there is no way to delete exactly $(n-k+1)^2$ cells to meet the condition, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then, output $n$ lines. The $i$-th line should contain a binary string $t_i$ of length $n$. The $j$-th character of $t_i$ is <span class="tex-font-style-tt">0</span> if cell $(i, j)$ is deleted, and <span class="tex-font-style-tt">1</span> otherwise.</p><p>If there are multiple solutions, you can output any of them.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \leq k \leq n \leq 1000$). </p><p>Then $n$ lines follow. The $i$-th line contains a binary string $s_i$ of length $n$. The $j$-th character of $s_i$ is <span class="tex-font-style-tt">1</span> if you can delete cell $(i, j)$, and <span class="tex-font-style-tt">0</span> otherwise.</p><p>It's guaranteed that the sum of $n^2$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, if there is no way to delete exactly $(n-k+1)^2$ cells to meet the condition, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then, output $n$ lines. The $i$-th line should contain a binary string $t_i$ of length $n$. The $j$-th character of $t_i$ is <span class="tex-font-style-tt">0</span> if cell $(i, j)$ is deleted, and <span class="tex-font-style-tt">1</span> otherwise.</p><p>If there are multiple solutions, you can output any of them.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,3,4,10,11,12,13,14,15
4
2 2
10
01
4 3
1110
0101
1010
0111
5 5
01111
10111
11011
11101
11110
5 2
10000
01111
01111
01111
01111
```




```output1
YES
01
11
YES
0011
1111
1111
1100
NO
YES
01111
11000
10000
10000
10000
```



## Note

<p>For the first test case, you only have to delete cell $(1, 1)$.</p><p>For the second test case, you could choose to delete cells $(1,1)$, $(1,2)$, $(4,3)$ and $(4,4)$.</p><p>For the third test case, it is no solution because the cells in the diagonal will always form a strictly increasing sequence of length $5$.</p>
