## Description

<div><p>Another dull quarantine day was going by when <span class="tex-font-style-it">BThero</span> decided to start researching matrices of size $n \times m$. The rows are numerated $1$ through $n$ from top to bottom, and the columns are numerated $1$ through $m$ from left to right. The cell in the $i$-th row and $j$-th column is denoted as $(i, j)$.</p><p>For each cell $(i, j)$ <span class="tex-font-style-it">BThero</span> had two values: </p><ol> <li> The cost of the cell, which is a single <span class="tex-font-style-bf">positive</span> integer. </li><li> The direction of the cell, which is one of characters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">U</span>. Those characters correspond to transitions to adjacent cells $(i, j - 1)$, $(i, j + 1)$, $(i + 1, j)$ or $(i - 1, j)$, respectively. No transition pointed outside of the matrix. </li></ol><p>Let us call a cell $(i_2, j_2)$ <span class="tex-font-style-it">reachable</span> from $(i_1, j_1)$, if, starting from $(i_1, j_1)$ and repeatedly moving to the adjacent cell according to our current direction, we will, sooner or later, visit $(i_2, j_2)$. </p><p><span class="tex-font-style-it">BThero</span> decided to create another matrix from the existing two. For a cell $(i, j)$, let us denote $S_{i, j}$ as a set of all reachable cells from it (including $(i, j)$ itself). Then, the value at the cell $(i, j)$ in the new matrix will be equal to the sum of costs of all cells in $S_{i, j}$. </p><p>After quickly computing the new matrix, <span class="tex-font-style-it">BThero</span> immediately sent it to his friends. However, he did not save any of the initial matrices! Help him to restore any two valid matrices, which produce the current one.</p></div><div class="input-specification"><p>The first line of input file contains a single integer $T$ ($1 \le T \le 100$) denoting the number of test cases. The description of $T$ test cases follows.</p><p>First line of a test case contains two integers $n$ and $m$ ($1 \le n \cdot m \le 10^5$).</p><p>Each of the following $n$ lines contain exactly $m$ integers — the elements of the produced matrix. Each element belongs to the segment $[2, 10^9]$.</p><p>It is guaranteed that $\sum{(n \cdot m)}$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if an answer does not exist, print a single word <span class="tex-font-style-tt">NO</span>. Otherwise, print <span class="tex-font-style-tt">YES</span> and both matrices in the same format as in the input.</p><ul> <li> The first matrix should be the <span class="tex-font-style-it">cost matrix</span> and the second matrix should be the <span class="tex-font-style-it">direction matrix</span>. </li><li> All integers in the <span class="tex-font-style-it">cost matrix</span> should be positive. </li><li> All characters in the <span class="tex-font-style-it">direction matrix</span> should be valid. No direction should point outside of the matrix. </li></ul></div>

## Input

<p>The first line of input file contains a single integer $T$ ($1 \le T \le 100$) denoting the number of test cases. The description of $T$ test cases follows.</p><p>First line of a test case contains two integers $n$ and $m$ ($1 \le n \cdot m \le 10^5$).</p><p>Each of the following $n$ lines contain exactly $m$ integers — the elements of the produced matrix. Each element belongs to the segment $[2, 10^9]$.</p><p>It is guaranteed that $\sum{(n \cdot m)}$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if an answer does not exist, print a single word <span class="tex-font-style-tt">NO</span>. Otherwise, print <span class="tex-font-style-tt">YES</span> and both matrices in the same format as in the input.</p><ul> <li> The first matrix should be the <span class="tex-font-style-it">cost matrix</span> and the second matrix should be the <span class="tex-font-style-it">direction matrix</span>. </li><li> All integers in the <span class="tex-font-style-it">cost matrix</span> should be positive. </li><li> All characters in the <span class="tex-font-style-it">direction matrix</span> should be valid. No direction should point outside of the matrix. </li></ul>





```input1
2
3 4
7 6 7 8
5 5 4 4
5 7 4 4
1 1
5
```




```output1
YES
1 1 1 1
2 1 1 1
3 2 1 1
R D L L
D R D L
U L R U
NO
```


