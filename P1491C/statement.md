## Description

<div><p>There is a trampoline park with $n$ trampolines in a line. The $i$-th of which has strength $S_i$.</p><p>Pekora can jump on trampolines in multiple passes. She starts the pass by jumping on any trampoline of her choice. </p><p>If at the moment Pekora jumps on trampoline $i$, the trampoline will launch her to position $i + S_i$, and $S_i$ will become equal to $\max(S_i-1,1)$. In other words, $S_i$ will decrease by $1$, except of the case $S_i=1$, when $S_i$ will remain equal to $1$. </p><p>If there is no trampoline in position $i + S_i$, then this pass is over. Otherwise, Pekora will continue the pass by jumping from the trampoline at position $i + S_i$ by the same rule as above.</p><p><span class="tex-font-style-bf">Pekora can't stop jumping during the pass until she lands at the position larger than $n$ (in which there is no trampoline)</span>. Poor Pekora!</p><p>Pekora is a naughty rabbit and wants to ruin the trampoline park by reducing all $S_i$ to $1$. What is the minimum number of passes she needs to reduce all $S_i$ to $1$?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5000$) — the number of trampolines.</p><p>The second line of each test case contains $n$ integers $S_1, S_2, \dots, S_n$ ($1 \le S_i \le 10^9$), where $S_i$ is the strength of the $i$-th trampoline.</p><p>It's guaranteed that the sum of $n$ over all test cases doesn't exceed $5000$.</p></div><div class="output-specification"><p>For each test case, output a single integer — the minimum number of passes Pekora needs to do to reduce all $S_i$ to $1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5000$) — the number of trampolines.</p><p>The second line of each test case contains $n$ integers $S_1, S_2, \dots, S_n$ ($1 \le S_i \le 10^9$), where $S_i$ is the strength of the $i$-th trampoline.</p><p>It's guaranteed that the sum of $n$ over all test cases doesn't exceed $5000$.</p>

## Output

<p>For each test case, output a single integer — the minimum number of passes Pekora needs to do to reduce all $S_i$ to $1$.</p>





```input1
3
7
1 4 2 2 2 2 2
2
2 3
5
1 1 1 1 1
```




```output1
4
3
0
```



## Note

<p>For the first test case, here is an optimal series of passes Pekora can take. (The bolded numbers are the positions that Pekora jumps into during these passes.)</p><ul> <li> $[1,4,\textbf{2},2,\textbf{2},2,\textbf{2}]$ </li><li> $[1,\textbf{4},1,2,1,\textbf{2},1]$ </li><li> $[1,\textbf{3},1,2,\textbf{1},\textbf{1},\textbf{1}]$ </li><li> $[1,\textbf{2},1,\textbf{2},1,\textbf{1},\textbf{1}]$ </li></ul><p>For the second test case, the optimal series of passes is show below.</p><ul> <li> $[\textbf{2},3]$ </li><li> $[1,\textbf{3}]$ </li><li> $[1,\textbf{2}]$ </li></ul><p>For the third test case, all $S_i$ are already equal to $1$.</p>
