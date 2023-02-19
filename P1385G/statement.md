## Description

<div><p>You are given a table $a$ of size $2 \times n$ (i.e. two rows and $n$ columns) consisting of integers from $1$ to $n$.</p><p>In one move, you can choose some <span class="tex-font-style-bf">column</span> $j$ ($1 \le j \le n$) and swap values $a_{1, j}$ and $a_{2, j}$ in it. Each column can be chosen <span class="tex-font-style-bf">no more than once</span>.</p><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> number of moves required to obtain permutations of size $n$ in both first and second rows of the table or determine if it is impossible to do that.</p><p>You have to answer $t$ independent test cases.</p><p>Recall that the permutation of size $n$ is such an array of size $n$ that contains <span class="tex-font-style-it">each integer</span> from $1$ to $n$ exactly once (the order of elements doesn't matter).</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of columns in the table. The second line of the test case contains $n$ integers $a_{1, 1}, a_{1, 2}, \dots, a_{1, n}$ ($1 \le a_{1, i} \le n$), where $a_{1, i}$ is the $i$-th element of the first row of the table. The third line of the test case contains $n$ integers $a_{2, 1}, a_{2, 2}, \dots, a_{2, n}$ ($1 \le a_{2, i} \le n$), where $a_{2, i}$ is the $i$-th element of the second row of the table.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case print the answer: <span class="tex-font-style-tt">-1</span> if it is impossible to obtain permutation of size $n$ in both first and the second rows of the table, or one integer $k$ in the first line, where $k$ is the <span class="tex-font-style-bf">minimum</span> number of moves required to obtain permutations in both rows, and $k$ <span class="tex-font-style-it">distinct</span> integers $pos_1, pos_2, \dots, pos_k$ in the second line ($1 \le pos_i \le n$) in <span class="tex-font-style-it">any order</span> — indices of columns in which you need to swap values to obtain permutations in both rows. If there are several answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of columns in the table. The second line of the test case contains $n$ integers $a_{1, 1}, a_{1, 2}, \dots, a_{1, n}$ ($1 \le a_{1, i} \le n$), where $a_{1, i}$ is the $i$-th element of the first row of the table. The third line of the test case contains $n$ integers $a_{2, 1}, a_{2, 2}, \dots, a_{2, n}$ ($1 \le a_{2, i} \le n$), where $a_{2, i}$ is the $i$-th element of the second row of the table.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case print the answer: <span class="tex-font-style-tt">-1</span> if it is impossible to obtain permutation of size $n$ in both first and the second rows of the table, or one integer $k$ in the first line, where $k$ is the <span class="tex-font-style-bf">minimum</span> number of moves required to obtain permutations in both rows, and $k$ <span class="tex-font-style-it">distinct</span> integers $pos_1, pos_2, \dots, pos_k$ in the second line ($1 \le pos_i \le n$) in <span class="tex-font-style-it">any order</span> — indices of columns in which you need to swap values to obtain permutations in both rows. If there are several answers, you can print any.</p>





```input1
6
4
1 2 3 4
2 3 1 4
5
5 3 5 1 4
1 2 3 2 4
3
1 2 1
3 3 2
4
1 2 2 1
3 4 3 4
4
4 3 1 4
3 2 2 1
3
1 1 2
3 2 2
```




```output1
0

2
2 3 
1
1 
2
3 4 
2
3 4 
-1
```


